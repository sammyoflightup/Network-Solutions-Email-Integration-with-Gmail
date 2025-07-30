# Gmail Integration – Custom Mail & Alias Setup

This repo documents how to connect external email accounts (custom or Gmail) to Gmail using POP/SMTP.

## ✅ Use Case

- Practice linking emails without owning a domain
- Learn Gmail as a mail client for business use
- Portfolio-ready mail integration workflow

---

## 🛠️ 1. Setup: Custom Email to Gmail

### Requirements

- Your domain email (e.g. info@yourdomain.com)
- Password and access to the email via webmail
- Gmail account

### Steps

#### A. Enable POP in Your Email

1. Login to your webmail (e.g., [mail.networksolutionsemail.com](https://mail.networksolutionsemail.com))
2. Navigate to **Settings** > **POP/IMAP**
3. Enable **POP** access
4. Save changes

#### B. Add Custom Email to Gmail (POP)

1. Go to Gmail → **Settings** → **Accounts and Import**
2. Under **Check mail from other accounts**, click **Add a mail account**
3. Enter your email (e.g., `you@domain.com`)
4. Choose **Import using POP3**
5. Enter the following:
Username: you@domain.com
Password: your password
POP Server: mail.domain.com (or pop.yourhost.com)
Port: 995
Use SSL: ✔️ Checked
Leave copy: ✔️ Optional

6. Click **Add Account**

#### C. Configure "Send As" (SMTP)

1. Gmail asks: *"Want to send mail as you@domain.com?"* → Choose **Yes**
2. Fill in:
SMTP Server: mail.domain.com
Port: 465 (SSL) or 587 (TLS)
Username: you@domain.com
Password: your password
Secure Conn: SSL or TLS

3. Gmail will send a verification email → copy the code
4. Paste code into Gmail setup

✅ You're now sending/receiving as your custom domain!

---

## 🛠️ 2. Setup: Gmail to Gmail (for practice)

### Requirements

- Your main Gmail account
- A second (test) Gmail account

### Steps

#### A. Enable POP in Second Gmail

1. Login to your second Gmail (the one you’ll receive from)
2. Go to **Settings** → **Forwarding and POP/IMAP**
3. Enable **POP for all mail**
4. Save changes

#### B. Add Second Gmail to Main Gmail

1. On your **main Gmail** → **Settings** → **Accounts and Import**
2. Click **Add mail account**
3. Enter the second Gmail address
4. Use these details:
Username: your-second@gmail.com
Password: your password or App Password
POP Server: pop.gmail.com
Port: 995
Use SSL: ✔️

#### C. Setup "Send As"

- Choose Yes → "Send mail as this account"
- SMTP Settings:
MTP Server: smtp.gmail.com
Port: 465 (SSL) or 587 (TLS)
Username: your-second@gmail.com
Password: Gmail password or App Password




📌 If you have 2FA, generate an **App Password** from [https://myaccount.google.com/apppasswords](https://myaccount.google.com/apppasswords)

✅ You now simulate a custom domain email experience using 2 Gmail accounts!

---

## 🧪 Optional Practice Tools

- [Zoho Mail](https://zoho.com/mail) – Free business email, good for real tests
- [Mailtrap.io](https://mailtrap.io) – Simulated dev inbox (for Laravel, PHP testing)

---




