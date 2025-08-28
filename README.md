# 🔒 Vulnerable Labs

⚠️ **Disclaimer:**  
This repository is created **only for educational and research purposes**.  
Do **NOT** deploy these vulnerable applications on public servers or use them against real targets.  
All labs here are intended to be run in a **local or virtualized environment** for safe learning.

---

## 📚 About
This repository contains a collection of intentionally vulnerable web applications and environments used for practicing **penetration testing**, **web security**, and **CTF-style challenges**. It is perfect for beginners who want to learn web vulnerabilities, exploitation techniques, and mitigation strategies in a safe environment.  
Included labs: DVWA (Damn Vulnerable Web Application), OWASP Juice Shop, bWAPP, and Mutillidae II.

---

## 🛠️ Prerequisites
- Docker (and optionally Docker Compose) installed on your machine.  
- Recommended: run inside a VM (VirtualBox/VMware/WSL2) and do **not** expose these services to the public internet.

---

## 🛠️ Setup Instructions

### DVWA (Damn Vulnerable Web Application)  
Contains vulnerabilities: SQL Injection, XSS, Command Injection, File Inclusion, CSRF, etc.

Run the following commands to start DVWA:

```bash
git clone https://github.com/digininja/DVWA.git
cd DVWA
docker-compose up -d
```

Access the app at: `http://localhost:8080`

---

### OWASP Juice Shop  
Modern vulnerable web app with realistic challenges.

Run the following command:

```bash
docker run --rm -p 3000:3000 bkimminich/juice-shop
```

Access the app at: `http://localhost:3000`

---

### bWAPP (Buggy Web Application)  
Covers 100+ web vulnerabilities for practice.

Run the following command:

```bash
docker run -d -p 8081:80 raesene/bwapp
```
Access the app at: `http://localhost:8081/install.php`

---

### Mutillidae II  
Vulnerable PHP/MySQL web application for training.

Run the following command:

```bash
docker run -d -p 8082:80 citizenstig/nowasp
```

Access the app at: `http://localhost:8082`

---

## 🚀 How to Use
1. Clone this repository.  
2. Choose the lab you want to practice with.  
3. Start it with Docker using the commands shown above.  
4. Explore vulnerabilities, practice exploitation, and learn mitigation techniques.  
5. Write a short writeup for each lab: what you tested, how you exploited it, and how to fix it.

---

## 🛡️ Recommended Setup & Safety
- Run in a **virtual machine** (VMware, VirtualBox, or WSL2).  
- Use a **pentesting distro** like Kali Linux for tools.  
- Make sure Docker containers are bound to `localhost` and are not reachable from external networks.  
- Always include a clear **disclaimer** and never use these labs against systems you do not own or have permission to test.

---

## 🎯 Next Steps (Ideas for the repo)
- Add a folder per lab with short writeups and screenshots.  
- Create a `docker-compose.yml` that can bring up selected labs together (optional).  
- Add "how to mitigate" section for each vulnerability you practice.  
- Add badges (status, license, topics) at the top for nicer appearance.

---

⭐ Happy hacking — and remember to learn responsibly!
