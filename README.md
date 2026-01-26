# Personal Friend Tracker & CRM

A lightweight, single-file web application designed to help you maintain relationships by tracking when you last interacted with friends and family. 

Built with privacy and simplicity in mind, it runs entirely in your browser with optional cloud syncing across devices.

![App Screenshot](image_bd4f2a.png)
## 🚀 Features

* **Interaction Logging:** Record notes, dates, and interaction types (In Person, Call, Message).
* **Smart Sorting:** Automatically sorts friends by who you haven't seen in the longest time.
* **Contextual Filters:** Filter the list to see the last time you saw someone *In Person* vs just *Messaged* them.
* **History Log:** View a complete timeline of interactions for every friend, with the ability to delete specific entries.
* **Search:** Instantly filter your list by name.
* **Dark Mode:** A clean, modern dark interface.
* **Mobile Responsive:** Optimized layout for usage on phones and desktops.
* **Data Backup:**
    * **Local:** Export/Import your data to a JSON file.
    * **Cloud Sync:** Sync data between devices (Phone/Laptop) using a free JSONBin.io account.

## 🛠️ How to Use

### Running Locally
1.  Download the `index.html` file.
2.  Open it in any web browser (Chrome, Safari, Firefox, etc.).
3.  Start adding friends!

### Hosting on GitHub Pages
Since this is a static site, you can host it for free using GitHub Pages:
1.  Go to your Repository **Settings**.
2.  Click on **Pages** (in the sidebar).
3.  Under **Branch**, select `main` (or `master`) and hit **Save**.
4.  Your app will be live at `https://<your-username>.github.io/<repo-name>/`.

## ☁️ Setting Up Cloud Sync (Cross-Device)

To sync data between your phone and computer, this app uses [JSONBin.io](https://jsonbin.io/) as a free storage backend.

1.  **Create an Account:** Go to [JSONBin.io](https://jsonbin.io/) and sign up (it's free).
2.  **Create a Bin:**
    * Click "Create Bin".
    * Add empty curly braces `{}` into the editor.
    * Click Create.
    * **Copy the "Bin ID"** (It looks like `65a123...`).
3.  **Get API Key:**
    * Go to the API Keys menu.
    * Create a new key.
    * **Copy the "X-Master-Key"**.
4.  **Connect the App:**
    * Open your Friend Tracker app.
    * Click the **Settings (⚙️)** icon in the top right.
    * Paste your **Bin ID** and **API Key**.
    * Click Save.

**How to Sync:**
* Click **⬆️ Upload** after making changes on one device.
* Click **⬇️ Download** when opening the app on a different device to fetch the latest data.

## 🔒 Privacy & Data

* **No Database:** This app does not run on a backend server.
* **Local Storage:** By default, all data is stored in your browser's `localStorage`.
* **Cloud Storage:** If you use the Sync feature, your data is stored in your private JSONBin.io bin. It is only accessible via your unique API Keys.

## 💻 Tech Stack

* **HTML5**
* **CSS3** (Flexbox & Responsive Grid)
* **JavaScript** (Vanilla ES6+)
* **Single File:** No build tools or frameworks (React/Vue) required.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
