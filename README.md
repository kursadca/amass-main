## 🛠️ amass-main - Featuring OWASP Amass

### Description

This repository offers a curated collection of tools for cybersecurity and penetration testing, with a **primary focus on external asset discovery and network mapping using the OWASP Amass Project.** Amass is an open-source tool that uses techniques like DNS, scraping, and active reconnaissance to find subdomains, IPs, and related assets. This makes it a critical tool for effective attack surface management.

⚠️ **Legal Disclaimer:** These tools are strictly intended for **legal and ethical purposes only**. The use of these tools against systems without explicit permission or for malicious intent is strictly prohibited and may violate local laws. All responsibility lies with the user.

### 🌟 Core Focus: OWASP Amass

Amass transforms scattered internal and external data into a complete picture of a target's exposed assets, aiding in deep reconnaissance.

| Amass Subcommand | Purpose |
| :--- | :--- |
| `amass intel` | Discover targets (domains, IPs, ASNs) for enumeration. |
| `amass enum` | Perform comprehensive enumeration and network mapping. |
| `amass viz` | Visualize enumeration results using graphs. |
| `amass track` | Track differences between enumerations over time. |
| `amass db` | Manipulate the Amass graph database. |

### 🚀 Getting Started

#### Prerequisites

To use Amass and other tools, a Linux-based OS (e.g., **Kali Linux**) and the **Go language** (for Amass installation) are highly recommended.

#### Installation (Amass)

If Amass is not pre-installed on your system, follow these steps:

1.  Ensure **Go** is installed.
2.  Install Amass using the Go tool:
    ```bash
    go install -v [github.com/owasp-amass/amass/v4/...@master](https://github.com/owasp-amass/amass/v4/...@master)
    ```
    *(Refer to the official OWASP Amass documentation for up-to-date installation methods.)*

#### Basic Usage Example

To perform a basic subdomain enumeration on a target domain:

```bash
amass enum -d example.com
