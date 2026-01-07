# 🔐 Reset Password – Supabase Recovery Page

A modern, mobile-friendly password reset page for **Supabase authentication**, designed to be hosted on **GitHub Pages** and opened directly from the Supabase recovery email link.

<img src="https://github.com/user-attachments/assets/c7663e0a-73c4-48cc-bd3f-872d313c140a" width="320" alt="Reset password preview" />

---

## ✨ Features

- ✅ Works with **Supabase Auth v2**
- 🔗 Opens directly from the **password recovery email**
- 🔐 Secure session detection
- 💪 Live password strength meter
- 📋 One-click password copy
- 🎲 Strong password generator
- 👁️ Show / hide password
- ⚠️ Caps-lock warning
- ⏱️ Session expiration timer
- 🎉 Success screen after update
- 📱 Mobile-optimized UI
- 🚀 Deep-link back to your Android app

---

## 🌍 Live Demo

Your page is live here:  
👉 **https://aliencodingjava.github.io/reset-password/**

---

## ⚙️ How it works

1. User taps **Reset password** link from Supabase email  
2. Supabase redirects to this page with a recovery session  
3. Page detects the session using `supabase-js`  
4. User sets a new password  
5. Password is updated via:
   ```js
   client.auth.updateUser({ password })
