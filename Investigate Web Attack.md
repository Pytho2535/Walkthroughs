![LetsDefend](https://img.shields.io/badge/LetsDefend-Walkthrough-blue)
![SOC Analyst](https://img.shields.io/badge/Role-SOC_Analyst-red)
![Cybersecurity](https://img.shields.io/badge/Focus-Cybersecurity-green)
# 🛡️ Investigate Web Attack – LetsDefend Walkthrough

---

## 🔍 Step-by-Step Investigation

---

### 🧩 1st Question
**Question: Which automated scan tool did attacker use for web reconnaissance?**

**🔎 Investigation:**
Checked for reconnaissance activity – looked for suspicious user agents.

![Analysis](https://github.com/user-attachments/assets/bfe71fc5-f067-4eeb-a5a4-d724f98f88a4)


Found entries with User-Agent: Nikto

![Answer](https://github.com/user-attachments/assets/ca0d2c93-d189-4bb2-9fe9-500928b525c1)


---

### 🧩 2nd Question
***Question: After web reconnaissance activity, which technique did attacker use for directory listing discovery?***

**🔎 Investigation:**
We can see a lot of "guessing" behavior, indicating brute force attempts.

![Analysis](https://github.com/user-attachments/assets/db1b81e0-f415-45d5-908b-4ca3ea1c4d2c)


This kind of guessing is referred to as directory brute force.

![Answer](https://github.com/user-attachments/assets/7555f068-7f1c-4557-a3dd-0c27ed544880)

---

### 🧩 3rd Question
***Question: What is the third attack type after directory listing discovery?***

**🔎 Investigation:**
We look further down and find numerous login attempts.

![Analysis](https://github.com/user-attachments/assets/c9fd67c6-c670-4eca-95dd-17deac26d8bd)


A large number of login requests suggest brute-force login attack.

![Answer](https://github.com/user-attachments/assets/7c47e62e-c618-428f-a6d6-c2ae9acf9b2d)

---

### 🧩 4th Question
***Question: Is the third attack successful?***

**🔎 Investigation:**
We review response codes and sizes to infer success of the attack.

![Analysis](https://github.com/user-attachments/assets/1a69939b-54e4-4de5-8f6e-93bea7871114)


Response code 302 and increased response size suggest the attack was successful.

![Answer](https://github.com/user-attachments/assets/aef88586-06ee-4646-a549-86d19ed39a04)

---

### 🧩 5th Question
***Question: What is the name of fourth attack?***

**🔎 Investigation:**
We observe commands directly in the URL – classic sign of code injection.

![Analysis](https://github.com/user-attachments/assets/11a3a543-e18f-4f6d-8278-d02750d0fd56)


![Answer](https://github.com/user-attachments/assets/4d0c81bb-54dc-4b76-a4fa-3406e34fcca4)

---

### 🧩 6th Question
***Question: What is the first payload for 4th attack?***

**🔎 Investigation:**
We look at the first payload.

![Analysis](https://github.com/user-attachments/assets/4523b231-c6e6-48fd-9fa2-ed6dba942011)

![Answer](https://github.com/user-attachments/assets/e0f1fe4b-8b58-4ce0-80b3-d0903c5118be)

---

### 🧩 7th Question
***Question: Is there any persistency clue for the victim machine in the log file ? If yes, what is the related payload?***

**🔎 Investigation:**
The question asks about persistence – did the attacker attempt to maintain access?

![Analysis](https://github.com/user-attachments/assets/86f8d458-6238-4952-acdd-faaed720e2db)

Indeed, the attacker created a user account: `hacker` with password `Asd123!!`

![Answer](https://github.com/user-attachments/assets/d85a0697-9b74-4134-9095-1f4478db8300)


---
