* **`!DOCTYPE.html`** → An intentionally vulnerable dark-mode XSS demo
* **`!DOCTYPE_safe.html`** → A secure version with input sanitization


# 🌐 XSS Demo: Vulnerable vs Safe

This repository demonstrates the difference between an **XSS-vulnerable web page** and a **secure, sanitized version**.
It is intended **for educational purposes only** to help understand the impact of cross-site scripting (XSS) and how to mitigate it.

---

## 📂 Project Structure

* **`!DOCTYPE.html`** → 🚨 *Vulnerable version*

  * Directly injects user input into the DOM with `innerHTML`
  * Allows execution of arbitrary scripts (XSS)

* **`!DOCTYPE_safe.html`** → 🛡️ *Safe version*

  * Sanitizes user input using a custom `escapeHTML` function
  * Prevents injected scripts from executing

---

## 🚀 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/xss-demo.git
   cd xss-demo
   ```

2. Open the files in a browser:

   * `!DOCTYPE.html` → to see the insecure version
   * `!DOCTYPE_safe.html` → to see the protected version

No server is required (pure HTML/CSS/JS).

---

## 📝 Learning Outcomes

* Understand how **XSS attacks** exploit unescaped user input.
* See how a simple **input sanitization function** can block such attacks.
* Learn best practices for **secure DOM manipulation**.

---

## 🔒 Mitigation Tips

* Always sanitize or escape user input.
* Use `.textContent` instead of `.innerHTML` where possible.
* Consider libraries like **DOMPurify** for stronger XSS protection.

---


Do you want me to also add **badges** (e.g., HTML5, security warning, MIT License) and a **demo screenshot** section to make the README look more professional?
