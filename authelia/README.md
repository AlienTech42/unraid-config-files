# 🔐 Authelia Setup (Unraid + Cloudflare Tunnel)

This repo contains the config files used in my Authelia setup video.

👉 Full video: https://youtu.be/LRFwjATqFdw

---

## 📂 Files Included

* configuration.yml → Main Authelia config
* users_database.yml → User login + password
* commands.txt → All the commands used in the video
* NGINX_script.txt → The script that gets added to NGINX Advanced tab or Settings gear

---

## ⚙️ Setup Steps (Important)

### 1. Generate Secrets

Run this in your Unraid terminal:

```
openssl rand -base64 32
```

Use this for:

* session.secret
* encryption_key
* jwt_secret

---

### 2. Generate Password Hash

Run:

```
docker run authelia/authelia:latest authelia crypto hash generate argon2 --password 'YourPassword'
```

Copy your password hash, then copy the output into:

`users_database.yml → password`

---

### 3. Update Your Domain

Replace all instances of:

```
yourdomain.com
```

With your actual domain.

---

### 4. Notification Setup

By default, this uses:

```
/config/notification.txt
```

For testing.

---

## ⚠️ Important Notes

* Do NOT reuse example secrets
* Do NOT leave default passwords
* Make sure your domain matches your Cloudflare setup

---

## 💬 Need Help?

👉 Discord: https://discord.gg/kst8fMPx4t

---

## 🧠 Free Unraid Getting Started Guide

👉 https://alientech42.kit.com/5e40652209

