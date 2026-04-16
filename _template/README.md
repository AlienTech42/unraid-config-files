# ⚙️ [SETUP NAME] (Unraid)

This repo contains the config files used in this setup.

👉 Full video: (PASTE VIDEO LINK)

---

## 📂 Files Included

* configuration.yml → Main config
* example.conf → Reverse proxy / app config
* notes.txt → Optional notes

*(Files will vary depending on the setup)*

---

## ⚙️ Setup Steps

### 1. Update Required Values

Before using these files, make sure you update:

* Domain names (`yourdomain.com`)
* IP addresses (`10.0.0.x`)
* Passwords / secrets

---

### 2. Generate Secrets (if required)

```bash
openssl rand -base64 48
```

Use for:

* API keys
* session secrets
* JWT secrets

---

### 3. Generate Password Hash (if required)

```bash
authelia crypto hash generate
```

Paste into the appropriate config file.

---

### 4. Apply the Config

* Place files in the correct Unraid directories
* Restart container/app
* Test access

---

## ⚠️ Important Notes

* Always review configs before using
* Never reuse example secrets
* Double-check your domain and proxy settings

---

## 💬 Need Help?

👉 Discord: https://discord.gg/kst8fMPx4t

---

## 🧠 Free Unraid Getting Started Guide

👉 https://alientech42.kit.com/5e40652209

---

## 👽 About

These are the same configs used in my videos.

Built for beginners.
Designed to actually work.

