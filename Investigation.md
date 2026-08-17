# Questions
## Question 1
While reviewing the forum server's logs, you notice traffic that doesn't match normal user behavior. What is the exact timestamp of the attacker's first attempt to exploit the forum application? (4 points)  
`YYYY-MM-DD HH:MM:SS`

---

## Question 2
Your analysis shows the attacker was able to export the application's database without ever authenticating. Which PHP file was abused to make this possible? (4 points)  
`file.php`

---

## Question 3
The attacker exploited a race condition by registering a "special" username with the administrator's password hash coming from the exported database. What was the exact username used for this registration as recorded in the database logs? (4 points)  
`XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX X XXXXXXXX`

---

## Question 4
Having gained administrative session cookies through the race condition, the attacker proceeded to reset the administrator's password. At what exact time did this password reset take place? (4 points)  
`YYYY-MM-DD HH:MM:SS`

---

## Question 5
As part of establishing a foothold, the attacker uploaded a PHP stager disguised as a legitimate file belonging to the forum. What is the full path on the filesystem where this first "stager" was stored? (4 points)  
`/var/…/full/path/to/file.ext`

---

## Question 6
To trigger the RCE, the attacker imported a malicious plugin. What was the pluginid assigned by the system to this first malicious plugin? (3 points)  
`integer`

---

## Question 7
As a result the malicious plugin enabled, triggering the stager to drop its webshell. At what exact time did the attacker first access the webshell successfully? (4 points)  
`YYYY-MM-DD HH:MM:SS`

---

## Question 8
Once the plugin was enabled, a persistent webshell appeared on the filesystem. What is the full path of this webshell file? (4 points)  
`/var/…/full/path/to/webshell.php`

---

## Question 9
From the webshell, the attacker wanted a more interactive session. What is the exact command they executed to upgrade their shell? (3 points)  
`Full Command Line`

---

## Question 10
At some point the attacker escalated their privileges on the host. At what exact time did this privilege escalation occur? (4 points)  
`YYYY-MM-DD HH:MM:SS`

---

## Question 11
With root-level access, the attacker used a specific utility to dump the entire database. At what exact time did this dump take place? (4 points)  
`YYYY-MM-DD HH:MM:SS`

---

## Question 12
Shortly after, the attacker exfiltrated the dump from the server. At what exact time did the exfiltration occur? (4 points)  
`YYYY-MM-DD HH:MM:SS`

---

## Question 13
Before leaving the system, the attacker dropped a text file in the root directory. What is the name of this file? (4 points)  
`file.ext`

---


# Indicators of Compromise (IOCs)
