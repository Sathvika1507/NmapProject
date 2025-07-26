# 🔍 Nmap Network Scanning Project

## 👤 Student Details
- **Name:** Sathvika Bogam  
- **Roll Number:** BT23ECE062  
- **Course:** B.Tech ECE  
- **Internship Title:** Network Security Intern  
- **Tool Used:** Nmap v7.97  
- **Platform:** macOS (Apple M1)

---

## 📌 Objective
To understand and perform a basic network scan using Nmap on a public IP (Google DNS: `8.8.8.8`) and identify open ports, services, and host information.

---

## 🛠️ Tools & Technologies
- **Nmap:** Network exploration and security auditing tool  
- **macOS Terminal:** For executing commands  
- **Homebrew:** Package manager used to install Nmap  

---

## 🚀 How to Run the Project

### ✅ Step 1: Install Nmap on macOS
If you haven't already, install Homebrew first:
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Then install Nmap:
```bash
brew install nmap
```

---

### ✅ Step 2: Verify Nmap Installation
Check the Nmap version to ensure it installed correctly:
```bash
/opt/homebrew/bin/nmap --version
```

Expected output:
```
Nmap version 7.97 ( https://nmap.org )
```

---

### ✅ Step 3: Run a Basic Nmap Scan
Scan Google's DNS server (`8.8.8.8`) using:
```bash
sudo /opt/homebrew/bin/nmap 8.8.8.8
```

_Note: `sudo` is used to run with elevated privileges._

---

### ✅ Step 4: Save Scan Results to a File
To save the output to a `.txt` file:
```bash
sudo /opt/homebrew/bin/nmap 8.8.8.8 > scan_result.txt
```

This creates a file called `scan_result.txt` in the current directory containing the scan results.

---

## 📄 Sample Output from Scan
```
Starting Nmap 7.97 ( https://nmap.org ) at 2025-07-26
Nmap scan report for dns.google (8.8.8.8)
Host is up (0.025s latency).
Not shown: 998 filtered tcp ports
PORT     STATE SERVICE
53/tcp   open  domain
443/tcp  open  https
```

---

## 📁 Project Structure
```
NmapProject/
├── README.md
├── scan_result.txt
├── Sathvika_Bogam_Nmap_Report.pdf (optional)
```

---

## ✅ Conclusion
This mini-project demonstrates:
- Installing Nmap on macOS
- Performing a basic port scan on a public IP
- Saving scan results for documentation

This forms a strong foundation for deeper exploration into network security and ethical hacking.

---

## 📚 References
- [Nmap Official Website](https://nmap.org)
- [Homebrew for macOS](https://brew.sh)
