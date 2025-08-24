# CloudSEK CTF 2025 - Writeup

## Challenge: Welcome Challenge - Flag 1

- **Category:** OSINT  
- **Points:** 50  

### Description

```
Astra Bank has been hit by a massive cyberattack. Their systems were breached, and the attackers left no clear trace behind. To uncover the truth, Astra Bank has called in CloudSEK, a well-known threat intelligence company.

During the investigation, CloudSEK analysts found a clue - the email address [suryanandanmajumder@gmail.com](mailto:suryanandanmajumder@gmail.com) was used by the attacker to carry out the breach.

Your mission is to continue the investigation from here. Follow the trail, dig deeper, and at every step you will discover a hidden secret text. Each secret you find must be submitted as proof that you are on the right path.

```

### Solution
Since this was an OSINT challenge, I began by looking for an email OSINT tool. I used [epieos.com](https://epieos.com/) and searched for the provided email address.  

From the results, I discovered services linked to the email, including a **Google Maps profile**. Checking that profile revealed a **review by the local guide**, which contained a GitHub name:

👉 [tuhin1729/tg-bot](https://github.com/tuhin1729/tg-bot)  

I navigated to the repository and explored the commit history. In the very first create commit of (`app.py`), I found the hidden flag.  

### Flag

``` 
CloudSEK{Flag\_1\_w3lc0m3\_70\_7h3\_c7f}

```


