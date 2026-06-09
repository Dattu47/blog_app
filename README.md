# 📝 Modern Flask Blog App

A modern, responsive multi-user blogging web application built with **Flask** and integrated with **Google Firebase (Cloud Firestore & Cloud Storage)**. It features user authentication, image uploads, post interactions (likes & comments), and a fully equipped administrative panel.

---

## ✨ Features

### 👤 User Authentication
* **Registration**: Secure sign-up with SHA-256 password hashing.
* **Session Login/Logout**: Adapts layout and capabilities dynamically depending on session state.

### ✍️ Blog Posting & Management
* **Post Creation**: Create posts with titles, formatted content, and custom image uploads.
* **Edit/Delete Posts**: Authors can modify or remove their own posts at any time.
* **Personal Library ("My Posts")**: A dedicated screen listing only your authored content.

### 💬 Engagement & Interactions
* **Likes**: Real-time counter allowing logged-in readers to express appreciation.
* **Comments**: Nested sub-collections linked to individual posts for open discussion threads.

### 🛡️ Administrative Dashboard
* **Content Moderation**: Administrators can delete any blog post.
* **User Management**: Administrators can delete user profiles, which cleanly purges all posts and comments written by them.

### 🎨 Premium UI/UX Design
* **Glassmorphism Styling**: Elegant dark navbar backdrop filter.
* **Modern Typography**: Integrated Google Font *Plus Jakarta Sans*.
* **Micro-interactions**: Lift-on-hover card animations and smooth inputs.

---

## 🛠️ Tech Stack
* **Backend**: Python, Flask, Firebase Admin SDK
* **Database**: Google Cloud Firestore (NoSQL document database)
* **Storage**: Local uploads directory / Firebase Cloud Storage
* **Frontend**: HTML5, Jinja2, Bootstrap 5, Font Awesome, Custom CSS3

---

## 🚀 Setup & Installation

Follow these steps to run the project locally on your machine:

### 1. Prerequisites
Ensure you have **Python 3.10+** installed on your system.

### 2. Clone the Repository
```bash
git clone https://github.com/Dattu47/blog_app.git
cd blog_app
```

### 3. Create & Activate a Virtual Environment
**On Windows:**
```bash
python -m venv venv
venv\Scripts\activate
```
**On macOS/Linux:**
```bash
python3 -m venv venv
source venv/bin/activate
```

### 4. Install Dependencies
```bash
pip install -r requirements.txt
```

### 5. Setup Firebase Credentials
1. Generate a new private key certificate file in JSON format from the **Firebase Console** (Project Settings > Service Accounts).
2. Save this file as `firebase_config.json` in the root folder of the project.

### 6. Run the Server
```bash
python app.py
```
Open your browser and visit: **[http://127.0.0.1:5000](http://127.0.0.1:5000)**