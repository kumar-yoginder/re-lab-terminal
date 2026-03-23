# 🖥️ RE-Lab Terminal

> An interactive malware reverse engineering terminal — built as a cyberpunk portfolio piece by [Yoginder Kumar](https://linkedin.com/in/kyogi), Security Researcher @ Trellix.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-▶%20Launch%20Terminal-00ffcc?style=for-the-badge&labelColor=0a0a0f)](https://kumar-yoginder.github.io/re-lab-terminal/)
[![GitHub Pages](https://img.shields.io/badge/Hosted%20on-GitHub%20Pages-181717?style=for-the-badge&logo=github)](https://kumar-yoginder.github.io/re-lab-terminal/)
![HTML](https://img.shields.io/badge/HTML-E34F26?style=flat-square&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Cyberpunk](https://img.shields.io/badge/Vibe-Cyberpunk-ff2d78?style=flat-square)

---

## `> preview`

```
yoginder@re-lab:~$ analyze agent_tesla.exe

  [+] static analysis: agent_tesla.exe
  ────────────────────────────────────────────────────
  file         agent_tesla.exe
  size         284 KB
  md5          a3f2c1d9e7b04561
  entry point  0x00401000
  packer       UPX 3.96
  entropy      6.21 (packed sections ~7.8)
  family       AgentTesla

  notable imports:
    ├─ WSAStartup
    ├─ HttpSendRequestA
    ├─ RegSetValueExA
    ├─ CryptAcquireContextA
    ├─ GetAsyncKeyState

  c2           103.45.67.89:4444
  yara rule    agent_tesla_v3
  ────────────────────────────────────────────────────
  next: pe agent_tesla.exe · mitre agent_tesla.exe · yara agent_tesla.exe
```

---

## `> help`

### Analyst
| Command | Description |
|---------|-------------|
| `whoami` | Analyst profile |
| `projects` | Open source tools |
| `certs` | Certifications & achievements |

### Samples
| Command | Description |
|---------|-------------|
| `ls samples` | List available malware samples |
| `analyze <name>` | Full static analysis report |
| `pe <name>` | PE header deep-dive (arch, timestamp, TLS, sections) |
| `entropy <name>` | Section entropy bar chart + packing verdict |
| `strings <name>` | Extract high-interest strings with offsets |
| `disasm <name>` | Disassembly snippet with technique annotations |

### Detection
| Command | Description |
|---------|-------------|
| `yara <name>` | Generate production-ready YARA rule |
| `ioc <name>` | Structured IOC report (hashes, network, host artefacts) |
| `c2 <name>` | C2 infrastructure + exfil analysis |
| `mitre <name>` | MITRE ATT&CK technique mapping |

### System
| Command | Description |
|---------|-------------|
| `history` | Command history |
| `clear` | Clear terminal |

**Tip:** Use `↑` / `↓` arrow keys to navigate command history.

---

## `> ls samples`

| Sample | Family | Size | Notable Technique |
|--------|--------|------|-------------------|
| `agent_tesla.exe` | AgentTesla | 284 KB | T1056.001 Keylogging |
| `mimidrv.sys` | Mimikatz Driver | 56 KB | T1003.001 LSASS Dump |
| `ransom_cl0p.bin` | Cl0p Ransomware | 1.2 MB | T1486 Data Encryption |
| `njrat.exe` | njRAT v0.7d | 112 KB | T1105 Ingress Tool Transfer |

> All samples are **simulated / educational** — no real malware is present.

---

## `> deploy`

This runs entirely in the browser — no backend, no dependencies.

```bash
# Clone
git clone https://github.com/kumar-yoginder/re-lab-terminal.git
cd re-lab-terminal

# Open locally
open index.html

# Or serve
python3 -m http.server 8080
```

**GitHub Pages:** Settings → Pages → Deploy from branch `main` → root `/`

Your terminal is live at `https://kumar-yoginder.github.io/re-lab-terminal/`

---

## `> about`

Built by **Yoginder Kumar** — Security Researcher with 4.5+ years in malware reverse engineering, detection engineering, and red teaming. Analyst of 111M+ malware samples.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-kyogi-0077B5?style=flat-square&logo=linkedin)](https://linkedin.com/in/kyogi)
[![X](https://img.shields.io/badge/X-@ekasunyaasta-000000?style=flat-square&logo=x)](https://x.com/@ekasunyaasta)
[![GitHub](https://img.shields.io/badge/GitHub-kumar--yoginder-181717?style=flat-square&logo=github)](https://github.com/kumar-yoginder)

---

## `> license`

MIT — fork it, theme it, add your own samples.
