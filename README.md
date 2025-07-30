# Network-Solutions-Email-Integration-with-Gmail
This project demonstrates how to integrate a business email hosted on Network Solutions with Gmail for both **sending and receiving** emails.

## Objective
To set up:
- Gmail to fetch emails from a Network Solutions inbox via POP3
- Gmail to send emails using SMTP on behalf of the domain email

---

## Requirements
- Gmail account
- Network Solutions email (e.g. you@yourdomain.com)
- Access to Webmail and SMTP/POP server info

---

## Configuration Steps

### 1. Enable POP on Network Solutions Webmail
- Log in to [mail.networksolutionsemail.com](https://mail.networksolutionsemail.com)
- Go to **Settings > POP/IMAP** and enable POP access

### 2. Add Account in Gmail for Receiving
- Go to Gmail → **Settings > Accounts and Import**
- Under "Check mail from other accounts", click **Add a mail account**
- Enter:
  - Email: `you@yourdomain.com`
  - POP3 server: `mail.yourdomain.com` (port 995 with SSL)
  - Username: Full email
  - Password: Email password

### 3. Configure Gmail to Send from Custom Email
- After adding, Gmail will prompt to set up sending
- SMTP server: `mail.yourdomain.com` (port 587 or 465)
- Use full email and password
- Confirm via verification link sent to inbox

---

## Outcome
After setup:
- Emails sent to `you@yourdomain.com` appear in your Gmail
- You can send as `you@yourdomain.com` from within Gmail
- Seamless management of business communication

---

## Notes
- Use **SSL/TLS** for security
- Create app password if 2FA is enabled
- Test send/receive after configuration

---

## Project Structure
This project contains:
email-integration-practice/
├─ README.md
├─ config-guide.pdf (optional if you want to attach screenshots or step-by-step)



---

## Security
Passwords are never stored in this repo. This is a **local-only demo** and for **learning/practice purposes only**.

---

## Author
**Samuel George**  
Practice Task for Upwork Simulation  
July 2025

