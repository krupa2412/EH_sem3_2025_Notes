
# 📄 File Permission Report – chmod 751

**Repository:** EH_sem3_2025_Notes  
**Directory:** 1st Assignment  
**Author:** Krupa Anna Chandy      
**Date:** 31 July 2025  
**Task:** Create a file and apply specific permissions using octal `751`

---

## 🛠️ Methodology

I created a file named `myfile.txt` using the `touch` command. I then changed its permissions using the `chmod` command with octal mode `751`. To verify the changes, I used `ls -l` to inspect the permission string and confirm each user class (owner, group, others) had the correct access levels.

### Commands Used:
```bash
touch myfile.txt
chmod 751 myfile.txt
ls -l myfile.txt
````

---

## 📸 Screenshots


<img width="555" height="291" alt="chmod_output" src="https://github.com/user-attachments/assets/2e752869-8701-4b76-b4a9-f265e2c58570" />

---

## 📊 Findings

### Result from `ls -l`:

```bash
-rwxr-x--x 1 user user 0 Jul 31 10:15 myfile.txt
```

This confirms:

| User Type | Permission | Explanation                      |
| --------- | ---------- | -------------------------------- |
| Owner     | `rwx` (7)  | Full access (read/write/execute) |
| Group     | `r-x` (5)  | Read and execute only            |
| Others    | `--x` (1)  | Execute only                     |

Octal `751` = `rwxr-x--x`

---

## 📌 Conclusions

* I learned how Linux assigns permissions using octal notation (`chmod`).
* Proper permission control is essential for security and functionality.
* The octal system is an efficient way to manage access rights for files and scripts.

---

## 💻 Code

```bash
# Create the file
touch myfile.txt

# Apply permissions
chmod 751 myfile.txt

# Verify
ls -l myfile.txt
```

---
