# Event Sign-In Kiosk

A professional, offline-capable sign-in system designed for clubs, classrooms, and events. This application runs directly in your web browser with no installation required.

[![Kiosk Visualization](https://img.youtube.com/vi/rki8POKA9rs/0.jpg)](https://youtu.be/rki8POKA9rs)

---

## 1. How to Download and Utilize

This application is designed to be portable and easy to run from any computer, including USB drives.

1.  **Download/Unzip**: Ensure you have the entire project folder saved on your computer or USB drive.
2.  **Launch**: Open the folder and double-click the file named **`sign.html`**.
    *   *Note: This will open in your default web browser (Chrome, Edge, Firefox, etc.).*
3.  **Kiosk Mode**: For the best professional experience, press **F11** on your keyboard to enter Fullscreen mode. This hides the browser bars and makes the app look like a dedicated program.

---

## 2. Functions of the Event Side

 The **Event Mode** is tailored for specific meetings, workshops, or guest speaker events.

*   **Topic & Interest Tracking**: Allows you to define specific meeting topics and custom interest tags for attendees to select.
*   **Rapid Attendee Entry**: streamlined form for First Name, Last Name, and Email Username.
*   **Officer Check-In**: A discrete/hidden field for officers to sign in using a secret 4-digit code.
*   **Live Statistics**: Real-time display of "Queued Attendees" and "Board Members Present" at the top of the screen.
*   **Duplicate Prevention**: Checks to ensure board members don't sign in multiple times.

---

## 3. How to Use the Event Side

1.  **Navigate**: From the Main Menu, click the large **Start Meeting** button.
2.  **Setup**:
    *   **Topic**: Enter the name of the event (e.g., "Weekly Workshop").
    *   **Interests**: (Optional) Enter comma-separated values (e.g., "Coding, Hardware, Design") to create clickable buttons for attendees.
    *   Click **Launch Kiosk**.
3.  **Attendee Interaction**:
    *   Attendees type their Name and Email Username.
    *   They click any relevant Interests.
    *   They click **Record Entry**.
    *   *Success Message*: A green confirmation appears briefly.
4.  **Officer Sign-In**:
    *   Officers tap the small input box in the top right of the instructions panel.
    *   Enter their 4-digit code and click the **Checkmark** button.

---

## 4. Functions of the Running Log (MakerSpace Mode)

The **Running Log** (defaulted as "MakerSpace Log") is designed for daily attendance tracking, such as open lab hours or library visits.

*   **Check-In / Check-Out**: Distinct buttons to track entry and exit times.
*   **Duration Tracking**: The system records the exact timestamp for both actions.
*   **Live Clock**: A large digital clock is displayed for convenience.
*   **Email Automation**: Automatically appends the student domain (e.g., `@student.monroecc.edu`) to usernames.

---

## 5. How to Use the Running Log

1.  **Navigate**: From the Main Menu, click the large **Log Mode** button (right side).
2.  **User Entry**:
    *   Enter First Name, Last Name, and Email Username.
3.  **Action**:
    *   Click **Check IN** (Green) when arriving.
    *   Click **Check OUT** (Red) when leaving.
4.  **Confirmation**: A pulsing message will confirm the action and clear the form for the next person.

---

## 6. Where to Find Settings and Config

Configuration is handled in two places:
1.  **In-App Settings**: Accessible via the **Gear Icon** responsible for immediate, temporary changes.
2.  **`config.js` File**: The physical file in the project folder responsible for **permanent** settings.

**Accessing In-App Settings:**
*   On the Main Menu, click the **Gear Icon** in the bottom right corner.
*   Enter the Admin PIN (Default: `1234`).

---

## 7. How to Access Config

To view or edit the raw configuration (useful if you forget your PIN):
1.  Navigate to the project folder on your computer.
2.  Right-click the file named **`config.js`**.
3.  Select **Open with > Notepad** (or any text editor).
4.  You can view `clubName`, `pin`, `officerCodes`, and `colors` directly here.

---

## 8. How to Change and Manipulate Config

**Method A: Using the App (Recommended for visual changes)**
1.  Go to **Settings** (Gear Icon -> PIN).
2.  **General**: Update Club Name, Log Mode Name, or Change PIN.
3.  **Appearance**: Click color boxes to adjust the theme.
4.  **Officer Codes**: Add new codes/roles or delete old ones.
5.  **Apply**: Click "Apply Changes" to test them instantly.
6.  **SAVE PERMANENTLY**:
    *   **CRITICAL STEP**: The browser cannot save to your computer directly due to security rules.
    *   Click the **Download Config** button.
    *   A new `config.js` file will download to your "Downloads" folder.
    *   **Move and Replace** the old `config.js` in your Kiosk folder with this new one.

**Method B: Editing the File Directly**
1.  Open `config.js` with Notepad.
2.  Edit the values inside the quotes (e.g., `"clubName": "My New Club"`).
3.  Save the file (Ctrl+S).
4.  Refresh the web page (`sign.html`) to see changes.

---

## 9. How to End Events and Export Files

To save your attendance data to an Excel file:

1.  **Exit Mode**: Click the **X** button in the top right corner of the Event or Log screen to return to the Main Menu.
2.  **Go to Settings**: Click the Gear Icon and enter PIN.
3.  **Data Management Panel**: Look for the "Data Management" section.
    *   **MakerSpace Logs**: Shows count of logs. Click **Export .xlsx** to save the daily log.
    *   **Pending Event Queue**: Shows count of event attendees. Click **Export .xlsx** to save the event attendance sheet.
    *   *Note: Using "Clear" helps reset the queue for the next event, but export first!*
