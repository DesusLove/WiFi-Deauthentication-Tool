# 📡 **Wi-Fi Deauthentication Tool**

---

## ⚠️ **Disclaimer**

> **This tool is provided for educational purposes only.**  
> It must only be used for **legitimate penetration testing** and **authorized security research** on networks you own or have explicit permission to test.
>
> Unauthorized use is **illegal** and may violate laws such as the **Computer Fraud and Abuse Act (CFAA)**, leading to criminal charges, penalties, and legal action.
>
> The author **shall not be held responsible** for any damages, misuse, or legal violations resulting from the use of this tool.  
> **Use at your own risk, with proper authorization, and in compliance with all applicable laws.**

---

## 📖 **Introduction**

**Wi-Fi Deauthentication Tool** is a **command-line utility** designed for educational and authorized security testing. It enables users to perform controlled Wi-Fi network analysis and deauthentication testing in **legal, ethical environments**.

> ✅ **Intended for:** Security researchers, penetration testers, educators, and network administrators.

---

## 🔧 **Features**

| Feature | Description |
|---------|-------------|
| 🔍 **Scan for Wi-Fi networks** | Discover nearby networks and view details (BSSID, channel, encryption) |
| 🎯 **Select a network for actions** | Choose a specific target network from scan results |
| 👤 **Deauthenticate a client** | Send deauth packets to a specific connected device |
| 👥 **Deauthenticate all clients** | Send deauth packets to all devices on a selected network |
| 📡 **Check Wi-Fi adapter status** | Verify monitor mode and interface status |
| 🔄 **Change adapter interface name** | Modify the wireless interface identifier |

---

## 📦 **Prerequisites**

### **System Requirements:**
- **Linux** environment (Kali, Ubuntu, etc.)
- **Wireless adapter** supporting monitor mode
- **Root/sudo privileges**

### **Tool Installation:**
```bash
# Install aircrack-ng suite
sudo apt update
sudo apt install aircrack-ng -y

# Alternative for Red Hat-based systems:
sudo yum install aircrack-ng
```

### **Verify Installation:**
```bash
which airodump-ng
which aireplay-ng
```

---

## 🚀 **Usage**

```bash
# 1. Clone/download the script
git clone <repository-url>
cd <repository-directory>

# 2. Make executable
chmod +x wifideauth.sh

# 3. Run with sudo (requires root for raw packet injection)
sudo ./wifideauth.sh

# 4. Follow interactive menu
```

### **Interactive Menu Example:**
```
[1] Scan for Wi-Fi networks
[2] Select target network
[3] Deauthenticate specific client
[4] Deauthenticate all clients
[5] Check adapter status
[6] Change interface name
[0] Exit
```

---

## 🛡️ **Legal & Ethical Usage**

### ✅ **Permitted Uses:**
- Testing **your own** wireless networks
- **Authorized** penetration testing with written consent
- **Educational demonstrations** in controlled labs
- **Security research** with IRB/ethics approval

### ❌ **Prohibited Uses:**
- Attacking networks **without permission**
- Disrupting **public or neighbor networks**
- Any form of **cyber harassment** or disruption
- **Commercial exploitation** without licensing

### 📜 **Compliance Requirements:**
- Obtain **written authorization** for all testing
- Document **scope and rules of engagement**
- Follow **responsible disclosure** practices
- Respect **privacy and data protection** laws (GDPR, CCPA, etc.)

---

## 📄 **License**

This project is licensed under the **MIT License**.  
See the [LICENSE](LICENSE) file for full details.

```
MIT License

Copyright (c) [Year] [Author]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

[...]
```

---

## ⚡ **Quick Start Commands**

```bash
# Install dependencies
sudo apt install aircrack-ng

# Enable monitor mode (example)
sudo airmon-ng start wlan0

# Run tool
sudo ./wifideauth.sh
```

---

## 🆘 **Troubleshooting**

| Issue | Solution |
|-------|----------|
| **"Interface not found"** | Check interface name with `iwconfig` |
| **Monitor mode fails** | Use `sudo airmon-ng check kill` |
| **No networks detected** | Ensure adapter supports 2.4GHz/5GHz |
| **Permission denied** | Run with `sudo` and verify group memberships |

---

## 🔗 **Related Resources**

- **[Official aircrack-ng docs](https://www.aircrack-ng.org/)**
- **[Wireless Pentesting Guide](https://www.wirelesshack.org/)**
- **[MITRE ATT&CK Framework](https://attack.mitre.org/techniques/T1562/008/)**

---

<div align="center">
  <sub>🔐 Built for education • ⚖️ Use legally • 🛡️ Test responsibly</sub>
</div>
