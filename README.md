# Attendance System (Render Deployed)

Live URL: **https://attendance-app-n1j7.onrender.com**

A lightweight **student attendance web app** built specifically for  
🎓 **Darshan University (B.Tech Batch 2024–2028)** students.  
It provides a fast, interactive roll-call interface for class batches **3A** and **3B**,  
with keyboard control, speech assist, and instant absentee summary.

---

## 👥 Project User Details

| Detail | Description |
|:-------|:-------------|
| **Institute** | Darshan University, Rajkot |
| **Course** | B.Tech (Computer Science & Engineering) |
| **Batch** | 2024 – 2028 |
| **Use Case** | For faculty and class representatives to mark daily attendance |
| **Classes Covered** | 3A and 3B |
| **Developed By** | Jeel Dobariya (DU Student) |
| **Academic Year** | 2025 – 26 |
| **Platform** | Web-based, accessible via Render deployment |

---

## ✨ Features

- **Batch Selection:** Toggle between *3A* / *3B* to show the correct student range.  
- **Dynamic Range Loading:**  
  - *3A:* Load 101–200 or 201–280  
  - *3B:* Load 301–429  
- **Interactive Cards:** Each student card shows Name, Roll No, and Enrollment No.  
- **Marking Controls:**  
  - ✅ *Mark All Present*  
  - ❌ *Mark All Absent*  
  - Individual click toggles focus and mark status  
- **Keyboard Shortcuts:** Use **↑ ↓ ← →** to navigate and mark quickly.  
- **Speech Assistance:** Audible roll-call with *speed control* and *on/off toggle*.  
- **Live Summary:** Real-time **Present / Absent counters**.  
- **Submission Output:** Displays the **Absent Roll Numbers** or “All Present!”  
- **Responsive UI:** Works on both desktop and mobile.  
- **404 Route:** Returns a simple “Page Not Found” message for invalid URLs.

> 💡 Student list reflects the **official DU 2025–26 roster (Batch 2024–2028)**.

---

## 🗂️ Folder Structure

```
attendance-app/
├── index.html        # UI, logic, student list, and functions
├── server.js         # Express server serving index.html
├── package.json      # Dependencies and start script
├── package-lock.json
└── student.js        # Backup student data file
```

---

## 🛠️ Tech Stack

- **Frontend:** HTML, CSS, Vanilla JavaScript  
- **Backend:** Node.js + Express  
- **Environment Config:** dotenv  

---

## ▶️ Run Locally

**Requirements:** Node.js ≥ 18

1️⃣ **Install dependencies**
```bash
cd attendance-app
npm install
```

2️⃣ **Create `.env` file**
```env
APP_NAME=Attendance App
PORT=3000
```

3️⃣ **Start the server**
```bash
npm start
```

Then open: [http://localhost:3000](http://localhost:3000)

---

## 🌐 Deployment on Render

Already deployed at 👉 **https://attendance-app-n1j7.onrender.com**

If redeploying:

| Setting | Value |
|----------|-------|
| **Environment** | Node |
| **Root Directory** | `attendance-app` |
| **Start Command** | `node server.js` |
| **Environment Vars** | `APP_NAME=Attendance App` (optional) |

---

## 🔌 Express Routes

| Method | Path | Description |
|:-------|:-----|:-------------|
| GET | `/` | Serves the main `index.html` |
| GET | `*` | 404 - Page Not Found handler |

---

## 🧭 How to Use

1. Choose your **batch (3A / 3B)**  
2. Load student list (by roll number range)  
3. Use checkboxes or keyboard arrows to mark attendance  
4. Toggle speech for voice readout  
5. Adjust speed if needed  
6. Click **Submit** to view absent list

---

## ⚙️ Environment Variables

| Variable | Description | Default |
|:----------|:-------------|:---------|
| `PORT` | Port for local server | `3000` |
| `APP_NAME` | Display name for app (console log) | `"Attendance App"` |

---

## 🧾 Example Output

After submission:
```
Absent Roll Numbers:
105, 113, 145, 176
```
If all present:
```
🎉 All students are present!
```

---

## 📜 License

Educational use only – developed for **Darshan University (B.Tech 2024–2028)** internal coursework.  
You may modify and reuse with attribution under the **MIT License**.

---

## 🙌 Credits

- Built by **Jeel Dobariya** (Darshan University)  
- Mentored and evaluated under DU Academic Curriculum 2025–26  
- Hosted using **Render Cloud Platform**

---

✅ **Final Render Deployment:**  
🔗 [https://attendance-app-n1j7.onrender.com](https://attendance-app-n1j7.onrender.com)
