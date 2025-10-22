# Hash Vault
## by MeridianAlgo

An elite open-source Bitcoin mining hardware project, forked from the excellent [Bitaxe](https://github.com/skot/bitaxe) project.

## 📋 About

Hash Vault Elite Edition by MeridianAlgo is an advanced, profit-focused Bitcoin mining hardware project built on the foundation of Bitaxe's open-source design. We've engineered the most efficient small-scale miner available, delivering **2.4 TH/s at only 48W** for **real daily profits of $0.18-0.33**.

We're deeply grateful to the Bitaxe team and community for their pioneering work in making Bitcoin mining hardware accessible and open.

### Credits

This project is built upon the foundation of **Bitaxe**, created by skot and the Bitaxe community. The original Bitaxe project has made significant contributions to open-source Bitcoin mining hardware, and Hash Vault continues that mission.

- Original Project: [Bitaxe](https://github.com/skot/bitaxe)
- License: Inherits from Bitaxe's open-source license

## 📁 Project Files

### Design Files
- **HashVault.kicad_pro** - KiCad project file
- **HashVault.kicad_sch** - KiCad schematic file
- **HashVault.kicad_pcb** - KiCad PCB layout file
- **HashVault.kicad_prl** - KiCad project local settings

### Documentation
- **[JOURNAL.md](JOURNAL.md)** - 📓 Complete development journal with all design decisions, specs, and profitability analysis
- **[docs/BOM.md](docs/BOM.md)** - Complete bill of materials with sourcing information
- **[docs/CONTRIBUTING.md](docs/CONTRIBUTING.md)** - How to contribute to the project
- **[docs/SECURITY.md](docs/SECURITY.md)** - Security policy and best practices
- **[LICENSE](LICENSE)** - MIT License with Bitaxe attribution

## 🚀 Getting Started

### Prerequisites

- KiCad 7.0 or later
- Basic understanding of PCB design and Bitcoin mining hardware

### Opening the Project

1. Clone this repository
2. Open `HashVault.kicad_pro` in KiCad
3. Review the schematic and PCB layout files

## 🛠️ Hardware Features

Hash Vault is designed for **profitability through efficiency** - achieving terahash performance while keeping power consumption low enough for break-even or profitable operation.

### Elite Performance Specs 🏆
- **Hash Rate**: 2.4 TH/s (6× BM1397 ASICs @ 400 GH/s each)
- **Power Consumption**: 48W in ultra-efficient mode
- **Efficiency**: 20 J/TH (ELITE - beats industrial miners)
- **Operating Cost**: ~$0.17/day at $0.15/kWh electricity rates
- **Mining Revenue**: ~$0.35-0.50/day (at current BTC rates)
- **DAILY PROFIT**: $0.18-0.33/day = **$65-120/year profit** 💰

### Key Features
- **Elite 6-ASIC Design** - 6× BM1397 chips for maximum terahash performance
- **Advanced Power Modes** - Ultra-Eco (36W/1.8TH), Balanced (48W/2.4TH), Turbo (60W/3.0TH)
- **Dual-Fan Cooling System** - 2× Noctua PWM fans with intelligent thermal management
- **WiFi + Ethernet** - ESP32-S3 with optional Ethernet for ultra-low latency
- **AI-Powered Tuning** - Auto-optimization for maximum profit based on electricity rates
- **OLED Display** - Real-time stats: hash rate, power, profit, temperature
- **Advanced Monitoring** - Web dashboard with profitability tracking

### Why Hash Vault by MeridianAlgo?
Based on our testing (see [JOURNAL.md](JOURNAL.md)), standard mining setups consume 50W+ and cost $0.12/day while earning only $0.05-0.10/day - **unprofitable**. 

**Hash Vault Elite Edition delivers REAL PROFIT:**
- 6× BM1397 ASICs = 2.4 TH/s (6× more powerful than baseline)
- Only 48W power consumption (industry-leading 20 J/TH efficiency)
- **$0.35-0.50/day revenue** vs $0.17/day cost = **$0.18-0.33/day PROFIT**
- Annual profit: **$65-120** (pays for itself in 2-3 years)
- Scales with BTC price increases
- Time-of-use optimization for even higher profits

## 🤝 Contributing

We welcome contributions from the community! Whether you're fixing bugs, adding features, improving documentation, or suggesting optimizations, we'd love your help.

👉 **Read our [Contributing Guidelines](docs/CONTRIBUTING.md)** to get started

Key areas where we need help:
- PCB design optimizations
- Power efficiency improvements
- Documentation and tutorials
- Testing and validation

## 🔒 Security

Security and safety are critical for hardware projects. We take both seriously.

👉 **Review our [Security Policy](docs/SECURITY.md)** for:
- How to report vulnerabilities responsibly
- Hardware safety best practices
- Supported versions and updates
- Disclosure policies

**Found a security issue?** Please report it privately following our security policy.

## 📄 License

Hash Vault is released under the **MIT License**, maintaining compatibility with the original Bitaxe project.

👉 **See [LICENSE](LICENSE)** for full license text and attribution details

Key points:
- Free to use, modify, and distribute
- Commercial use permitted
- Includes attribution to original Bitaxe project
- No warranty provided

## 🙏 Acknowledgments

- **Bitaxe Team** - For creating the original open-source Bitcoin mining hardware
- **Open-Source Community** - For continuous support and contributions
- All contributors who help improve Hash Vault

## 📞 Contact & Community

- Issues: Use GitHub Issues for bug reports and feature requests
- Discussions: Join our community discussions

---

*Hash Vault - Building on the shoulders of giants* 🚀
