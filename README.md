# Instagram Sharing Bot 🚀

An advanced automation bot for Instagram that helps with **Reels, Posts, and Stories sharing with smart scheduling**.  
This project is designed to simplify content management on Instagram by allowing automated posting, multi-account management, and proxy-supported safe automation.  

---

## 🔑 Features
- Automatic **Reels, Posts, and Stories uploading**
- Smart **post scheduling** with time-based automation
- **Multi-account management** via `accounts.txt`
- **Proxy support** for safe and secure automation
- Simple **user-friendly interface**
- Session-based **secure login**
- Full **logging system** (`log.txt`) for monitoring

---

## 🛠️ Technologies Used
- **C#** for core logic
- **SQL** for account/session & schedule storage
- **HTML, CSS, JavaScript** for UI

---

## ⚙️ How It Works (System Overview)

1. **Media Source (Folder Structure) — Manual Placement Required**
   Users **manually place** media files into these folders:
   - `Gonderi` → Standard Instagram posts (images/videos)
   - `Hikaye` → Instagram stories
   - `Reels` → Instagram reels (vertical videos)

   The bot **does not download or fetch media automatically**. It only posts the files you have manually added to these folders.

2. **Login & Authentication**
   - Credentials are read from `accounts.txt` in the format:
     ```
     username:password
     ```
   - Proxies (if used) are loaded from `proxy.txt` in the format:
     ```
     http://username:password@server:port
     ```
   - Secure session-based login is established and reused.

3. **Scheduling Module**
   - You can set a date/time for each post.
   - All schedules are stored in the SQL database for accuracy.

4. **Automation Engine**
   - At the scheduled time, the bot uploads the selected content.
   - Content type (Post, Story, Reels) is determined by the folder you placed it in.
   - Proper formatting is applied (e.g., vertical for Reels).

5. **Multi-Account Handling**
   - Supports multiple accounts via `accounts.txt`.
   - Each account can run with or without a proxy from `proxy.txt`.

6. **Reports & Logs**
   - All activity is written to `log.txt`.
   - Includes successful uploads, failed attempts, and proxy usage.

---

## 📸 Screenshots  

| Login | Main Screen | Start |
|-------|-------------|-------|
| <img width="420" height="257" alt="Login" src="https://github.com/user-attachments/assets/f24a87e5-fb42-467d-9485-e82c6689663d" /> | <img width="420" height="290" alt="MainScreen" src="https://github.com/user-attachments/assets/aecb3faa-2dd9-41a3-ac70-956defc12ea0" /> | <img width="420" height="290" alt="Start" src="https://github.com/user-attachments/assets/8b0fcc9d-8cce-4c38-acfd-0ddbd32f0559" /> |

---

## ⚙️ Setup Guide (Kurulum Rehberi)

1. **Download & Install**
   - Download the release and extract it into a working directory.

2. **Prepare Folders (Manual)**
   - Create or use the folders below and **manually copy** your media files:
     - `Gonderi` → images/videos for standard posts
     - `Hikaye` → media for stories
     - `Reels` → vertical videos for reels
   - The bot will only post **what you manually placed** in these folders.

3. **Account Configuration**
   - Open `accounts.txt`
   - Add accounts in the format:
     ```
     username:password
     ```

4. **Proxy Setup (Optional)**
   - Open `proxy.txt`
   - Add proxies in the format:
     ```
     http://username:password@server:port
     ```
   - Leave it empty if you don’t use proxies.

5. **Run the Bot**
   - Launch the program.
   - Choose the mode (Post / Story / Reels) and scheduling options.
   - Start automation.

6. **Check Logs**
   - All actions and errors are written to `log.txt`.

---

## ⚠️ Note
This is a **paid project**.  
Source code is **not publicly available** here. The repository only shows project details, system workflow, and screenshots.

---

## 📬 Contact
You can reach me on the following platforms:  

- [TikTok](https://www.tiktok.com/@furkan.gulsen?lang=tr-TR)  
- [Instagram](https://www.instagram.com/furkan.gulsen.01/)  
- [Bionluk](https://bionluk.com/crstyal)  
- [LinkedIn](https://www.linkedin.com/in/furkan-g%C3%BCl%C5%9Fen-53413137b/)  
