# 🔍 Useful Google Dorks for Bug Bounty Hunters  

I will make some modifications to it in the future. ✅

This list contains some **commonly used Google Dorks** that bug bounty hunters leverage to find **sensitive information**.  
>  Replace `target.com` with the actual domain you are testing.  

---

## 📌 Google Dorks Cheat Sheet

| 🏷️ Category | 🔎 Google Dorks |
|-------------|----------------|
| **Discovering Exposed Files** | `intitle:"index of" site:target.com` <br> `filetype:log inurl:log site:target.com` <br> `filetype:sql inurl:sql site:target.com` <br> `filetype:env inurl:.env site:target.com` |
| **Finding Sensitive Directories** | `inurl:/phpinfo.php site:target.com` <br> `inurl:/admin site:target.com` <br> `inurl:/backup site:target.com` <br> `inurl:wp- site:target.com` |
| **Exposed Configuration Files** | `filetype:config inurl:config site:target.com` <br> `filetype:ini inurl:wp-config.php site:target.com` <br> `filetype:json inurl:credentials site:target.com` |
| **Discovering Usernames & Passwords** | `intext:"password" filetype:log site:target.com` <br> `intext:"username" filetype:log site:target.com` <br> `filetype:sql "password" site:target.com` |
| **Finding Database Files** | `filetype:sql inurl:db site:target.com` <br> `filetype:sql inurl:dump site:target.com` <br> `filetype:bak inurl:db site:target.com` |
| **Exposed Git Repositories** | `inurl:".git" site:target.com` <br> `inurl:"/.git/config" site:target.com` <br> `intitle:"index of" ".git" site:target.com` |
| **Finding Publicly Exposed Emails** | `intext:"email" site:target.com` <br> `inurl:"contact" intext:"@target.com" -www.target.com` <br> `filetype:xls inurl:"email" site:target.com` |
| **Discovering Vulnerable Web Servers** | `intitle:"Apache2 Ubuntu Default Page: It works" site:target.com` <br> `intitle:"Index of /" "Apache Server" site:target.com` <br> `intitle:"Welcome to nginx" site:target.com` |
| **Finding API Keys** | `filetype:env "DB_PASSWORD" site:target.com` <br> `intext:"api_key" filetype:env site:target.com` <br> `intext:"AWS_ACCESS_KEY_ID" filetype:env site:target.com` |
| **Exposed Backup Files** | `filetype:bak inurl:backup site:target.com` <br> `filetype:zip inurl:backup site:target.com` <br> `filetype:tgz inurl:backup site:target.com` |

---


