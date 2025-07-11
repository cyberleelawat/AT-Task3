# AT-Task3
# 🔐 Task 3: Password Cracking using John the Ripper

👨‍💻 **Internship Program:** Alfido Tech – Cybersecurity Internship  
🙋‍♂️ **Intern Name:** Virendra Kumar  
🗂️ **Task Name:** Brute-force Password Cracking using John the Ripper  
📅 **Task Number:** Task 3

---

## 🎯 Task Objective
To perform a brute-force password cracking attack on a given MD5 hash using **John the Ripper** and extract the original plaintext password using a wordlist.

---

## 🧰 Tools Used

| Tool              | Purpose                                           |
|-------------------|---------------------------------------------------|
| **John the Ripper** | Password cracking engine                         |
| **Kali Linux**     | Operating system used for penetration testing     |
| **rockyou.txt**    | Common password dictionary (wordlist)             |

---

## 🧪 Steps Performed

### 1️⃣ Create a Hash File

A file named `hash.txt` was created and the MD5 hash was added to it.

```bash
nano hash.txt
```
#### Paste the hash value (e.g. 827ccb0eea8a706c4c34a16891f84e7b)
### 2️⃣ Run John the Ripper with Wordlist
```john --wordlist=/usr/share/wordlists/rockyou.txt hash.txt```
#### John started processing the hash against the wordlist.

### 3️⃣ Show the Cracked Password
```john --show hash.txt```

### ✅ Result
🎉 Password successfully cracked!
- Cracked Hash: 827ccb0eea8a706c4c34a16891f84e7b
- Plaintext Password: 12345

### 💡 What I Learned
- How password hashes are stored and processed
- The importance of strong, unpredictable passwords
- The effectiveness of common tools like John the Ripper in ethical hacking
- Basics of brute-force and dictionary-based attacks

