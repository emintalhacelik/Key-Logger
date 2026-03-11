# C# Keylogger (Educational Project)

## ⚠️ Disclaimer

This project was developed **strictly for educational and academic purposes**.
It demonstrates how **global keyboard hooks** work in Windows applications and how keystroke data can be processed programmatically.

The author **does not support or encourage any illegal use** of this software.
If this project is used for **malicious, unethical, or illegal activities**, the **author is not responsible** for any consequences.

Always use this project **only in controlled environments and with proper permission**.

---

## 📌 Project Description

This project is a **C# Windows Forms keylogger** created to demonstrate how keyboard input can be captured globally using the Windows API.

The application listens for specific keyboard events and records typed characters.
After collecting a certain number of keystrokes, the captured data is automatically **sent to a Telegram bot** using the Telegram Bot API.

The program runs **silently in the background** without showing a visible window.

---

## ⚙️ Features

* Global keyboard hook implementation
* Captures:

  * Alphabetic characters
  * Turkish characters (Ğ, Ü, Ş, İ, Ö, Ç)
  * Numbers
  * Special keys (Enter, Backspace, Space, etc.)
* Supports **Caps Lock detection**
* Automatically logs typed characters
* Sends collected keystrokes to a **Telegram bot**
* Runs in the background without displaying a UI
* Sends logs after **50 keystrokes**

---

## 🧠 How It Works

1. The program initializes a **global keyboard hook** using the `user32.dll`.
2. Specific keys are added to a **hooked keys list**.
3. When a key is pressed:

   * The key event is captured.
   * The corresponding character is added to a log string.
4. After **50 characters**, the log is sent to a **Telegram chat** using the Telegram Bot API.
5. The log is then reset and the process continues.

---

## 📡 Telegram Integration

The application sends captured keystrokes via the **Telegram Bot API**.


This allows remote monitoring of logged keystrokes.

---

## 🖥️ Technologies Used

* **C#**
* **.NET Windows Forms**
* **Windows API (user32.dll)**
* **Telegram Bot API**

---

## 📚 Educational Purpose

This project demonstrates:

* Windows keyboard hooking
* Event-driven programming
* Handling keyboard input programmatically
* Sending HTTP requests
* Basic remote logging techniques

It can be useful for studying:

* Cybersecurity concepts
* Malware analysis
* Keylogging detection techniques
* Windows API interaction

---

## ⚠️ Legal Notice

Keyloggers can be considered **malware** if used without user consent.

Before using or modifying this project, ensure that you:

* Use it **only in a lab or educational environment**
* Have **explicit permission** on any system where it is executed
* Follow **local laws and regulations**

The author **assumes no liability** for misuse.

---

## 👤 Author

**Emin Talha Celik**

---

## 📄 License

This project is released for **educational purposes only**.
Use responsibly.
