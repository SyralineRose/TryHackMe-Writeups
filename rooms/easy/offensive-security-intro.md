# Offensive Security Intro  

**Difficulty**: Easy  
**Tags**: Offensive Security, Enumeration, Web, dirb, gobuster  
**Date Completed**: 09-08-2025 

---

## 🔍 Overview  
This room introduces the fundamentals of offensive security — the attacker’s perspective.  
It covers the **attack lifecycle** (recon → enumeration → exploitation → post-exploitation) and provides hands-on exposure to common enumeration tools.  

---

## 📝 Notes  

### Attack Lifecycle Recap  
- **Reconnaissance** → collecting basic info about the target.  
- **Enumeration** → digging deeper into open services, hidden directories, and users.  
- **Exploitation** → using discovered vulnerabilities to gain access.  
- **Post-Exploitation** → escalating privileges and maintaining access.  

### Tools Encountered  
- **`dirb`** → a web content scanner that brute-forces directories and files on web servers using a wordlist.  
  - Example: `dirb http://target/ /usr/share/wordlists/common.txt`  
  - Helps uncover hidden directories or admin panels.  
- **`gobuster`** (looked at via husband’s notes) → similar to `dirb` but faster and more flexible.  
  - Example: `gobuster dir -u http://target/ -w /usr/share/wordlists/common.txt`  
  - Uses Go’s concurrency to speed up brute-forcing.  

### Observations  
- It was useful to see how both tools work toward the same goal (finding hidden content).  
- `dirb` felt more straightforward for me as a beginner, while `gobuster` looked faster and had more options.  
- This reinforced the idea that enumeration is about persistence — checking everything you can.  

---

## 🧩 Key Takeaways  
- Offensive security follows a **structured methodology**, not random guessing.  
- Enumeration tools like `dirb` and `gobuster` are essential for uncovering hidden web content.  
- Understanding multiple tools for the same task is valuable. Sometimes speed matters, sometimes simplicity does.  

---

## 🎯 Results  
- Completed all tasks and captured the room’s flag ✅  
