# 📁 1st Assignment - Directory Enumeration Report

**Repository:** `EH_sem3_2025_Notes`  
**Directory:** `1st Assignment`  
**Date:** 31 July 2025  
**Author:** Krupa Anna Chandy  
**Target:** http://testphp.vulnweb.com

---

## 🛠️ Tools Used

- **DIRB** – Web content scanner for discovering directories
- **Gobuster** – Fast, multi-threaded directory brute-forcer
- **Wordlist Used:** `/usr/share/wordlists/dirb/common.txt`

---

## 🔍 Methodology

Directory brute-force was conducted using `dirb` and `gobuster` to enumerate hidden and sensitive directories on the test target.

### Commands Used:
```bash
# Using DIRB
dirb http://testphp.vulnweb.com /usr/share/wordlists/dirb/common.txt

# Using Gobuster
gobuster dir -u http://testphp.vulnweb.com -w /usr/share/wordlists/dirb/common.txt -t 50
