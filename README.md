# Intro To Red Team — HackTheBox Course Notes

![Platform](https://img.shields.io/badge/Platform-HackTheBox-9FEF00?logo=hackthebox&logoColor=black)
![Type](https://img.shields.io/badge/Type-Course-blueviolet)
![Track](https://img.shields.io/badge/Track-Red%20Team-red)
![Status](https://img.shields.io/badge/Status-In%20Progress-yellow)
![Started](https://img.shields.io/badge/Started-2026--10--25-informational)

> My notes, commands and lab walkthroughs from the HackTheBox **Intro To Red Team** course.
> Lab answers are hidden behind spoiler sections. Try them yourself first.

---

## 📑 Table of Contents
- [Overview](#-overview)
- [Learning Roadmap](#️-learning-roadmap)
- [Progress Tracker](#-progress-tracker)
- [Module Notes](#-module-notes)
- [Lab Writeups](#-lab-writeups)
- [Cheatsheets](#-cheatsheets)
- [Key Takeaways](#-key-takeaways)

---

## 🧭 Overview

| Item | Detail |
|------|--------|
| Course | Intro To Red Team |
| Platform | HackTheBox |
| Enrolled | 2026-10-25 |
| Completed | _TBD_ |
| Certificate | _TBD_ |

---

## 🗺️ Learning Roadmap

```mermaid
flowchart LR
    A([📚 Enrolled]) --> B[Easy Linux boxes<br/>Cap · Sau · GoodGames · …]
    B --> C[Easy Windows boxes<br/>Jerry · Driver · Cicada]
    C --> D[Medium AD boxes<br/>Certified · Administrator]
    D --> E([🏁 Course complete])

    style A fill:#1b2a4a,stroke:#9FEF00,color:#fff
    style B fill:#14301a,stroke:#9FEF00,color:#9FEF00
    style C fill:#1b2a4a,stroke:#9FEF00,color:#fff
    style D fill:#2a1b3a,stroke:#b57edc,color:#fff
    style E fill:#1b2a4a,stroke:#9FEF00,color:#fff
```

> 15 machines total — mostly Easy Linux, ramping to two Medium Windows Active Directory boxes.

---

## ✅ Progress Tracker

**Boxes rooted: 1 / 15**

| # | Machine | Difficulty | OS | Writeup | Status |
|---|---------|-----------|-----|---------|--------|
| 1 | Cap | Easy | Linux | [writeups/cap.md](writeups/cap.md) | ✅ Done |
| 2 | Jerry | Easy | Windows | — | ⬜ Not started |
| 3 | Sau | Easy | Linux | — | ⬜ Not started |
| 4 | GoodGames | Easy | Linux | — | ⬜ Not started |
| 5 | Devvortex | Easy | Linux | — | ⬜ Not started |
| 6 | Paper | Easy | Linux | — | ⬜ Not started |
| 7 | Writeup | Easy | Linux | — | ⬜ Not started |
| 8 | Precious | Easy | Linux | — | ⬜ Not started |
| 9 | Driver | Easy | Windows | — | ⬜ Not started |
| 10 | BoardLight | Easy | Linux | — | ⬜ Not started |
| 11 | Cicada | Easy | Windows | — | ⬜ Not started |
| 12 | TwoMillion | Easy | Linux | — | ⬜ Not started |
| 13 | SteamCloud | Easy | Linux | — | ⬜ Not started |
| 14 | Certified | Medium | Windows | — | ⬜ Not started |
| 15 | Administrator | Medium | Windows | — | ⬜ Not started |

Legend: ⬜ Not started · 🟨 In progress · ✅ Done

---

## 📝 Module Notes

<details>
<summary><b>1. _Section name_</b></summary>

**Concepts**
- 

**Commands**
```bash
# 
```

<details>
<summary>🚩 Click to reveal lab answer</summary>

`answer here`

</details>
</details>

---

## 🧪 Lab Writeups

Full interactive machine walkthroughs completed during the course.

| Machine | Difficulty | Foothold | Privesc | Writeup |
|---------|-----------|----------|---------|---------|
| Cap | Easy | IDOR → pcap FTP creds | `cap_setuid` on python3.8 | [writeups/cap.md](writeups/cap.md) |

---

## 📋 Cheatsheets

- [cheatsheets/commands.md](cheatsheets/commands.md): commands collected throughout the course

---

## 💡 Key Takeaways

- 

---

<sub>Notes for educational purposes only. Only test systems you're authorized to attack.</sub>
