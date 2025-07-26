# Smart-Conference-Management-System

Smart Conference Management with Node‑RED automates live event speaker transitions, media playback, and attendee agenda updates via a one‑click dashboard. Deployed at iUG IBM Conference 2025, it uses JSON schedules and supports extensions like AI‑powered announcements.

---

## 📦 Deployment on Server

Since Node‑RED is already installed on your Rotown server, no local setup is needed. Simply upload the project files and start the service.

1. **Upload files with WinSCP**
   - Open **WinSCP** and connect to your Rotown server via SFTP or SCP.
   - Drag and drop the project folder (containing `flows.json`, `schedule.json`, `public/`, `docs/`, etc.) into your desired directory on the server (e.g., `/home/username/smart-conference`).

2. **Start the Node‑RED service**
   - SSH into your server:
     ```bash
     ssh username@your-server-ip
     ```
   - Navigate to the project directory and start Node‑RED:
     ```bash
     cd /home/username/smart-conference
     node-red
     ```
   - Ensure the service runs continuously (use `pm2`, `systemd`, or Docker, per your server setup).

3. **Access the application**
   - **Dashboard:** `http://your-server-ip:1880/ui`
   - **Public agenda:** `http://your-server-ip:1880/agenda`

---

## 🖼️ Verifying Uploaded Photos & Screenshots

Your `docs/` folder and image files have already been uploaded via WinSCP. To display them in this README, include the following Markdown references for your two screenshots:

```markdown
![Control Dashboard](./docs/1.PNG)
*The Node‑RED dashboard UI showing sound, video, and session controls.*

![Node-RED Flow](./docs/1751742951818.jpg)
*The core Node‑RED flow chart handling event timing and media triggers.*
```

Once these lines are in place, your images (`1.PNG` and `1751742951818.jpg`) will render automatically when viewed on GitHub or any Markdown previewer.

---

## ⚙️ Configuration

- **`schedule.json`** – Define event sessions, times, speakers, media URLs.
- **Environment Variables (if needed):**
  - `MEDIA_PATH` – Directory for media assets

---

## 🤝 Contributing

Contributions are welcome! Fork, branch, commit, and open a PR.

## 📄 License

MIT License

---

> **Meena Chand** · mchand@eoguk.com
