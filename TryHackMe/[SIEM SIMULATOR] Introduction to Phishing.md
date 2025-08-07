# TryHackMe – [Introduction to Phishing] Walkthrough
 
**Difficulty:** [Beginner]  
**Date completed:** [07.08.2025]

---

## 1. Lab Objective

Learn how to use SOC Simulator by completing your first scenario. Close all True Positive alerts to pass!

---

## 2. Walkthrough

### First Two Alerts
<img width="1877" height="879" alt="1" src="https://github.com/user-attachments/assets/b7ce2186-194d-4bc2-9a0a-9723fa70e6e0" />


After i got my first two alerts, i claimed them, opened playbook, and read what should i do <img width="1877" height="892" alt="2" src="https://github.com/user-attachments/assets/78897fd9-af17-495e-8994-303355920115" />

Then i discovered that there is splunk, which is very cool, because it gives us real possibility to learn it in practice<img width="1880" height="898" alt="3" src="https://github.com/user-attachments/assets/d8ed82f1-407c-441e-b08e-1edc41919b6d" />

After discovering what tools i have, i opened my Virtual Machine and proceed to check links attached to these email alerts
<img width="1917" height="912" alt="5" src="https://github.com/user-attachments/assets/51f59b22-4849-46bb-9c1d-042d5a37a5d7" />
It seems to be non-malicious which is good for us.

<img width="541" height="268" alt="image" src="https://github.com/user-attachments/assets/4cc44e22-5e22-4611-acb7-3cf59d74b3ee" />

We got 3 more alerts, so we prioritize the High Severity one.
<img width="1917" height="916" alt="7" src="https://github.com/user-attachments/assets/998a604d-2dd8-4590-88c4-408a4890d9a5" />

We can see that on the first glance it already looks suspicious
<img width="1917" height="916" alt="8" src="https://github.com/user-attachments/assets/cb8d0377-5d7a-4869-9908-677d9ad6138c" />

As usual we check the link in the email
<img width="1917" height="916" alt="9" src="https://github.com/user-attachments/assets/4a4d6aad-cb26-4a0e-aeca-c68a491a169d" />
It is indeed malicious, but we earlier saw that the action was blocked so we dont have to escalate it.

Now we check last two alerts
<img width="1917" height="916" alt="12" src="https://github.com/user-attachments/assets/4a703f8b-936b-4934-9dea-d694e7b16d55" />
First red flag that we can see is the sign of urgency in the email, then we see another suspicious link, so we check both links in both mails which are malicious and close these alerts.

And now we finished everything, all alerts were treated properly, we can see quick personal review of our actions and reports, which i find very cool.
Thanks for reading.

