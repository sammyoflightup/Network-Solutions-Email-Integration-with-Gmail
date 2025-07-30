#  Network Solutions Email Integration with Gmail

This project demonstrates how to integrate a business email hosted on **Network Solutions** with **Gmail** for both **sending and receiving** emails securely.

---

##  Overview

- Connects Network Solutions email to Gmail  
- Secure configuration with SSL  
- Custom "Send mail as" setup  
- PDF documentation included  

---

## Objective

To set up:
- Gmail to **fetch emails** from a Network Solutions inbox via **POP3**
- Gmail to **send emails** using **SMTP** on behalf of the domain email  

---

##  Requirements

- Gmail account  
- Network Solutions email (e.g., `you@yourdomain.com`)  
- Access to Webmail and SMTP/POP settings  

---

## Screenshots

> Use the following screenshots to ensure you're on the right page during each step.

### 1. Enable POP on Network Solutions Webmail  
![Enable POP on Webmail](images/webmail-pop-enable.png)

### 2. Add Account in Gmail for Receiving  
![Gmail POP3 Setup](images/gmail-pop3-setup.png)

### 3. Configure Gmail to Send Emails via SMTP  
![Gmail SMTP Setup](images/gmail-smtp-setup.png)

---

## Expected Outcome  
![Email Integration Working](images/email-working.png)

---

##  Configuration Steps

### 1. Enable POP on Network Solutions Webmail
- Go to: [mail.networksolutionsemail.com](https://mail.networksolutionsemail.com)  
- Navigate to **Settings > POP/IMAP**
- Enable **POP access**

---

### 2. Add Account in Gmail for Receiving
- Go to Gmail → **Settings > Accounts and Import**  
- Under "Check mail from other accounts", click **Add a mail account**
- Enter the following details:
  - **Email**: `you@yourdomain.com`
  - **POP3 server**: `mail.yourdomain.com`  
  - **Port**: `995`  
  - **Use SSL**: Yes  
  - **Username**: Full email address  
  - **Password**: Your email password  

---

### 3. Configure Gmail to Send from Custom Email
- After adding the account, Gmail prompts to configure **"Send mail as"**
- Use the following SMTP settings:
  - **SMTP server**: `mail.yourdomain.com`
  - **Port**: `587` or `465`  
  - **Username**: Full email address  
  - **Password**: Email password  
- Gmail will send a verification email — click the link to confirm  

---

## Result
After setup:
- Gmail will receive mail sent to `you@yourdomain.com`
- You can send mail **as your business email** from Gmail
- Everything is managed from one inbox  

---

## Project Structure
mail-integration-practice/    ← This is your repo folder
├── README.md                 ← Your main README file
├── config-guide.pdf          ← The PDF guide you referenced
└── images/                   ← Folder for all screenshots used in README
    ├── webmail-pop-enable.png
    ├── gmail-pop3-setup.png
    ├── gmail-smtp-setup.png
    └── email-working.png



---

## Security
Passwords are never stored in this repo. This is a **local-only demo** and for **learning/practice purposes only**.

---

## Author
**Samuel George**  
Practice Task for Upwork Simulation  
July 2025

