# Easy Sign-In App

Welcome! This is a simple, ready-to-use sign-in system for your club, classroom, or event. It runs directly in your web browser—**no installation required.**

---

## 🚀 Quick Start (30 Seconds)

1.  **Keep it together**: Make sure this folder is unzipped and saved on your computer (or USB drive).
2.  **Open the App**: Double-click the file named **`sign.html`**.
3.  **Go Fullscreen**: Press **F11** on your keyboard to make it look like a professional kiosk.

That's it! You are ready to go.

---

## ⚙️ How to Customize

Want to change the club name, colors, or passwords? You can do it all inside the app!

1.  **Click the Gear Icon** ⚙️ (Bottom right corner).
2.  **Enter the Admin PIN**: The default is `1234`.
3.  **Change Settings**:
    - **Club Name**: Type your organization's name.
    - **Colors**: Click the color boxes to pick a theme.
    - **PIN**: Change the code to something secret.
4.  **Save Your Changes (Important!)**:
    - Click **Apply** to test them.
    - To make them **Permanent**:
        1. Click **Download Config**.
        2. A new `config.js` file will download.
        3. **Move/Replace** the old `config.js` in your folder with this new one.
        *If you skip this, your settings will reset when you close the window!*

---

## 📅 How to Use

### 1. Meeting Mode (For Events)
Use this for specific meetings (e.g., "Guest Speaker", "Weekly Meeting").
- Click **Start Meeting**.
- Enter a Topic (optional).
- Users sign in with their Name.
- At the end, go to **Settings > Data Management** to download the attendance list.

### 2. Check-In Mode (For Daily Use)
Use this for a library, lab, or study hall where people come and go.
- Click the **Log Mode** button (e.g., "MakerSpace Log").
- Users can **Check In** (Green) and **Check Out** (Red).
- The system tracks exactly how long they stayed.

---

## ❓ Common Questions

**"I changed the name, but it went back to default!"**
You probably didn't replace the config file. Because this runs in a browser standard security prevents it from saving directly to your hard drive. You **must** download the new `config.js` and overwrite the old one.

**"I forgot my PIN!"**
Don't worry. Right-click the `config.js` file and choose **Open with > Notepad**. You can see your PIN inside text that looks like `"pin": "..."`.

**"Do I need WiFi?"**
Nope! It works completely offline. (However, connecting to the internet once helps load the icons and fonts).
