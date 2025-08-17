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

1. **Media Source (Folder Structure)**  
   Users place media files into specific folders:  
   - `Gonderi` → Standard Instagram posts  
   - `Hikaye` → Instagram stories  
   - `Reels` → Instagram reels  

   The bot scans these folders and prepares content automatically.  

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
   - Users can assign date/time for each post.  
   - All schedules are stored in the SQL database for accuracy.  

4. **Automation Engine**  
   - At the scheduled time, the bot uploads content automatically.  
   - Content type (Post, Story, Reels) is detected by folder.  
   - Correct formatting is applied (e.g., vertical for Reels).  

5. **Multi-Account Handling**  
   - Supports unlimited accounts via `accounts.txt`.  
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
   - Download the project release files.  
   - Extract them into a working directory.  

2. **Folder Preparation**  
   - Place your media files into the respective folders:  
     - `Gonderi` → Standard Instagram posts  
     - `Hikaye` → Stories  
     - `Reels` → Reels videos  

3. **Account Configuration**  
   - Open `accounts.txt`  
   - Add your accounts in the format:  
     ```
     username:password
     ```  

4. **Proxy Setup (Optional)**  
   - Open `proxy.txt`  
   - Add your proxies in the format:  
     ```
     http://username:password@server:port
     ```  
   - If not using proxies, leave the file empty.  

5. **Run the Bot**  
   - Launch the program.  
   - Login sessions will be created automatically.  
   - Choose scheduling options for posts/reels/stories.  

6. **Check Logs**  
   - All activity is saved in `log.txt`.  
   - Errors and successful posts can be tracked here.  

---

## ⚠️ Note
This is a **paid project**.  
Source code is **not publicly available** here. The repository only shows project details, system workflow, and screenshots.  

---

## 📬 Contact
For collaboration or inquiries, please reach out via GitHub profile.  
