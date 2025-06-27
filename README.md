# 🔥 Task 4 – UFW Firewall Configuration on Linux

> ✅ **Objective**: Learn how to configure and test basic firewall rules to allow/block network traffic using UFW (Uncomplicated Firewall) on Linux.

---

## 🛠️ Tools & Environment
- 🐧 **Operating System**: Linux (Kali/Ubuntu)
- 🔐 **Firewall Used**: UFW (Uncomplicated Firewall)
- 🔧 **Testing Tool**: Telnet, SSH

---

## ⚙️ Steps Performed

### 1️⃣ Install & Enable UFW
```bash
sudo apt install ufw -y
sudo ufw enable
sudo ufw status verbose
sudo ufw deny 23
sudo apt install telnet -y
telnet localhost 23  # Should show 'connection refused'
sudo ufw allow 22
sudo apt install openssh-server -y
sudo systemctl start ssh
sudo systemctl enable ssh
ssh localhost  # Should connect successfully
sudo ufw delete deny 23
sudo ufw status verbose
```


🧠 Key Concepts Covered
Firewall Rules ✅

UFW Commands ✅

Port Blocking & Allowing ✅

Telnet & SSH Testing ✅

Network Traffic Filtering ✅

