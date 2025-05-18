# kali_linux_toolkit_dataset
A machine-readable JSONL dataset of offensive security tools from Kali Linux — complete with command syntax, categories, flags, and references.
# Kali Linux Tools Dataset

A comprehensive and structured dataset of common offensive security tools available in **Kali Linux**, including usage commands, flags, descriptions, categories, and official documentation links.

This dataset is designed to support cybersecurity training, red team automation, LLM fine-tuning, and terminal assistants for penetration testers.

---

## 📁 Dataset Format

Each entry is a JSON object and stored in `.jsonl` (JSON Lines) format. This structure is ideal for machine learning pipelines and programmatic use.

### Fields:

| Field            | Description                                                             |
|------------------|-------------------------------------------------------------------------|
| `tool`           | Name of the Linux tool (e.g., `nmap`, `sqlmap`)                         |
| `command`        | A real-world example command                                            |
| `description`    | Human-readable explanation of what the command does                    |
| `category`       | Type of tool or use case (e.g., Networking, Exploitation, Web)         |
| `use_case`       | Specific purpose of the command (e.g., port scanning, password cracking)|
| `flags`          | Important flags used in the command                                     |
| `os`             | Operating system (`Linux`)                                              |
| `reference_link` | URL to official documentation or man page                               |

---

## 🧪 Example Entry

```json
{
  "tool": "sqlmap",
  "command": "sqlmap -u http://example.com --dbs",
  "description": "Enumerate databases on a vulnerable web application.",
  "category": "Web Application",
  "use_case": "SQL injection testing",
  "flags": ["-u", "--dbs"],
  "os": "Linux",
  "reference_link": "http://sqlmap.org/"
}
✅ Key Features

    ✅ Covers widely-used tools: nmap, hydra, sqlmap, burpsuite, aircrack-ng, wireshark, etc.

    ✅ Multiple real-world command examples per tool

    ✅ Cross-categorized where tools serve multiple purposes

    ✅ Ready for use in LLM training, cybersecurity education, and CLI helpers

🔍 Use Cases

    Fine-tuning AI models (LLMs) for cybersecurity and terminal tools

    Building red team knowledge bases or documentation bots

    Creating terminal assistant tools and cheat sheets

    Teaching ethical hacking through command-line exercises

📚 Categories Covered

    Networking

    Web Application Testing

    Exploitation

    Password Cracking

    Wireless Attacks

    System Forensics

    Sniffing & Spoofing

⚠️ Legal Notice

This dataset is provided for educational, research, and ethical security testing purposes only. Use of these tools and commands in unauthorized environments may be illegal.
📜 License

This dataset is released under the MIT License.
🙌 Contributions

Contributions are welcome! Feel free to submit PRs to add tools, improve descriptions, or fix errors.
📫 Maintainer

Created by: sunnythakur
GitHub: github.com/sunnythakur25
Contact: sunny48445@gmail.com
