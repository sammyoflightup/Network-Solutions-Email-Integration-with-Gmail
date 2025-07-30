# Gmail Integration – Custom Mail & Alias Setup

This repo documents how to connect external email accounts (custom or Gmail) to Gmail using POP/SMTP.

## Use Case

- Practice linking emails without owning a domain
- Learn Gmail as a mail client for business use
- Portfolio-ready mail integration workflow

---

##  1. Setup: Custom Email to Gmail

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

You're now sending/receiving as your custom domain!

---

##  2. Setup: Gmail to Gmail (for practice)

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

 If you have 2FA, generate an **App Password** from [https://myaccount.google.com/apppasswords](https://myaccount.google.com/apppasswords)

You now simulate a custom domain email experience using 2 Gmail accounts!
Step 1
![step 1](https://github.com/user-attachments/assets/cfe6c706-d1dc-41c0-892b-987fc4a8ecd9)
![step 2](https://github.com/user-attachments/assets/61afa773-be26-4d11-b2c9-3027c4060040)
![step 3](https://github.com/user-attachments/assets/286b3a93-e602-47a2-b663-aa28c5390b69)
![step 4](https://github.com/user-attachments/assets/3be96a7b-bc9e-4b38-824c-eea393b0e8c2)
![step 5](https://github.com/user-attachments/assets/e5794431-4517-4296-80d8-8d0121f8d29c)

Step 2
![2nd gmail step 1](https://github.com/user-attachments/assets/85286fff-562e-4669-81fe-aa53f90a3338)
![2nd email step 2](https://github.com/user-attachments/assets/44d0fa8a-33f1-407e-92b1-80cb0fa11122)
![2nd email step 3](https://github.com/user-attachments/assets/9d22b1e5-1471-46d5-8f26-12a0f04d7a1b)
![2 email step 4](https://github.com/user-attachments/assets/56f5e70f-ba1b-4dc2-9e80-7ddb77b55b1e)
![2nd gmail step 5](https://github.com/user-attachments/assets/d0d5af6b-d0c6-4321-ac9b-f0f7778909e2)
![2nd email step 6](https://github.com/user-attachments/assets/977d0780-90f1-48d4-b80f-3ca5372be34b)
![2nd email step 7](https://github.com/user-attachments/assets/3329c9d1-8ab1-470f-9f49-60a1d046445b)
---

##  Optional Practice Tools

- [Zoho Mail](https://zoho.com/mail) – Free business email, good for real tests
- [Mailtrap.io](https://mailtrap.io) – Simulated dev inbox (for Laravel, PHP testing)

---




