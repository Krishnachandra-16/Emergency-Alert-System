<div align="center">

# 🛡️ Guardian Elite

### Advanced Emergency Response & Tactical Command System

<p align="center">

<img src="https://img.shields.io/badge/Flutter-3.x-02569B?style=for-the-badge&logo=flutter"/>
<img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python"/>
<img src="https://img.shields.io/badge/Flask-Backend-black?style=for-the-badge&logo=flask"/>
<img src="https://img.shields.io/badge/SQLite-Database-003B57?style=for-the-badge&logo=sqlite"/>
<img src="https://img.shields.io/badge/JWT-Authentication-orange?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Platform-Android-success?style=for-the-badge&logo=android"/>
<img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge"/>

</p>

### 🚨 Because Every Second Counts.

*A modern real-time emergency response ecosystem that empowers users and emergency responders through live location tracking, forensic evidence collection, intelligent monitoring, and an interactive Tactical Command Center.*

---

⭐ **If you find this project useful, consider giving it a Star!**

</div>

---

# 📖 Overview

Guardian Elite is a **production-inspired emergency response platform** designed to improve safety during emergency situations.

Unlike traditional SOS applications that only send alerts, Guardian Elite creates an entire emergency ecosystem where responders receive continuous live intelligence including:

- 📍 Real-time GPS Tracking
- 🎙 Audio Evidence Recording
- 🔋 Device Battery Monitoring
- 📡 Continuous Location Streaming
- 🛰 Tactical Dashboard
- 🏥 Nearby Hospital Detection
- 👮 Nearby Police Detection
- 🔐 Rescue PIN Authentication

The project consists of three major components:

```
📱 Flutter Mobile App
        │
        ▼
⚙ Flask REST Backend
        │
        ▼
🛰 Tactical Command Dashboard
```

Together these components provide complete situational awareness during emergencies.

---

# ✨ Features

## 📱 Mobile Application

### 🚨 Emergency SOS

- One Tap SOS Activation
- Instant Live Tracking
- Emergency Session Creation
- Automatic Backend Synchronization

---

### 📍 Live GPS Tracking

- High Accuracy GPS
- Continuous Location Updates
- Background Tracking
- Live Dashboard Synchronization

---

### 🎙 Audio Evidence

- Automatic Recording
- Evidence Preservation
- Continuous Upload Support
- Forensic Collection

---

### 🚨 Emergency Utilities

- Loud Emergency Siren
- Flashlight Strobe
- Battery Monitoring
- GPS Status Monitoring

---

### 🔒 User Safety

- Secure Login
- JWT Authentication
- Rescue PIN Protection
- Protected Emergency Stop

---

# 🛰 Tactical Command Center

Designed for emergency responders with a real-time tactical interface.

Features include:

✅ Interactive Leaflet Map

✅ Live GPS Marker

✅ SOS Monitoring

✅ Emergency Timeline

✅ Device Status

✅ Live Battery Percentage

✅ Audio Evidence Viewer

✅ User Information

✅ Nearby Hospitals

✅ Nearby Police Stations

✅ Movement History

✅ Stealth Mode

---

# 🔐 Security

Guardian Elite implements multiple layers of protection.

- JWT Authentication
- Password Hashing
- Rescue PIN Verification
- Secure REST APIs
- Session Validation
- Protected Dashboard Endpoints

---

# 🏗 System Architecture

```text
                ┌──────────────────────────┐
                │    Flutter Mobile App    │
                └────────────┬─────────────┘
                             │
                       HTTPS REST API
                             │
                JWT Authentication Layer
                             │
                ┌────────────▼─────────────┐
                │      Flask Backend       │
                └────────────┬─────────────┘
                             │
             ┌───────────────┼──────────────┐
             │                               │
     SQLite Database                Tactical Dashboard
             │                               │
             └──────────Live Updates─────────┘
```

---

# 🛠 Tech Stack

| Layer | Technology |
|------------|----------------|
| Mobile App | Flutter |
| Backend | Flask |
| Programming | Python |
| Database | SQLite |
| Maps | Leaflet.js |
| Authentication | JWT |
| API | REST |
| Tunnel | Ngrok |
| Frontend | HTML CSS JavaScript |

---

# 📂 Project Structure

```
Guardian-Elite/
│
├── app.py
├── requirements.txt
├── README.md
│
├── instance/
│      emergency_system.db
│
├── templates/
│      dashboard.html
│
├── static/
│      css/
│      js/
│
├── emergency_mobile/
│      android/
│      ios/
│      lib/
│      assets/
│      pubspec.yaml
│
└── uploads/
```

---

# 🚀 Installation

## Clone Repository

```bash
git clone https://github.com/krishnachandra-16/Guardian-Elite.git
```

Move into the project directory

```bash
cd Guardian-Elite
```

---

## Backend Setup

Install Python packages

```bash
pip install flask flask-sqlalchemy flask-cors flask-bcrypt pyjwt
```

Start the backend

```bash
python app.py
```

The backend starts at

```
http://localhost:5000
```

---

## Flutter Setup

Move into Flutter project

```bash
cd emergency_mobile
```

Install packages

```bash
flutter pub get
```

Run application

```bash
flutter run
```

---

# 🌍 Global Deployment using Ngrok

Open another terminal

```bash
ngrok http 5000
```

You'll receive something similar to

```
https://abcd-123.ngrok-free.app
```

Copy this URL.

Open

```
lib/api_service.dart
```

Replace

```dart
static const String baseUrl =
"https://YOUR-NGROK-URL.ngrok-free.app";
```

Save the file.

Restart Flutter.

---
# 🚀 Running the System

Guardian Elite follows a **3-terminal architecture**. To ensure all services communicate correctly, launch them in the following order.

---

## 🖥️ Terminal 1 — Start Backend

Run the Flask server.

```bash
python app.py
```

You should see output similar to:

```
Running on http://127.0.0.1:5000
```

---

## 🌍 Terminal 2 — Start Ngrok

Expose the backend to the internet.

```bash
ngrok http 5000
```

Example output

```
Forwarding

https://abcd-123.ngrok-free.app
```

Copy this forwarding URL and update:

```
lib/api_service.dart
```

```dart
static const String baseUrl =
"https://abcd-123.ngrok-free.app";
```

---

## 📱 Terminal 3 — Run Flutter

Navigate into the Flutter project.

```bash
cd emergency_mobile

flutter pub get

flutter run
```

The mobile application is now connected to the live backend.

---

# 📱 Application Workflow

```text
User launches app
        │
        ▼
Secure Login
        │
        ▼
User presses SOS
        │
        ▼
Emergency Session Created
        │
        ▼
GPS Tracking Starts
        │
        ▼
Audio Recording Starts
        │
        ▼
Backend Receives Live Data
        │
        ▼
Dashboard Displays Live Information
        │
        ▼
Responder Monitors User
        │
        ▼
SOS Ends Using Rescue PIN
```

---

# 🛰 Dashboard Features

The Tactical Dashboard provides emergency responders with a real-time operational view.

## 🗺 Interactive Map

- Live GPS Marker
- Automatic Refresh
- User Movement Tracking
- Interactive Zoom
- Street Map

---

## 📍 Live Tracking

- Real-Time Coordinates
- Last Seen Time
- Device Online Status
- Continuous GPS Updates

---

## 🚨 SOS Information

- SOS Status
- Trigger Time
- Duration
- User Information

---

## 🎙 Audio Evidence

- Emergency Audio Recording
- Evidence Download
- Timeline Synchronization

---

## 🔋 Device Monitoring

- Battery Percentage
- Charging Status
- GPS Status
- Connection Health

---

## 🏥 Nearby Emergency Services

Automatically scans nearby:

- Hospitals
- Police Stations

using OpenStreetMap Overpass API.

---

## 👁 Stealth Mode

The dashboard supports **Stealth Mode**.

This hides all interface cards and displays only the interactive map, making it easier for responders to focus on live tracking.

---

# 📡 REST API Overview

| Endpoint | Method | Description |
|-----------|--------|-------------|
| `/register` | POST | Register new user |
| `/login` | POST | Authenticate user |
| `/activate_sos` | POST | Trigger SOS |
| `/deactivate_sos` | POST | Stop SOS |
| `/location` | POST | Send live GPS updates |
| `/dashboard` | GET | Retrieve dashboard data |
| `/profile` | GET | User profile |
| `/profile` | PUT | Update profile |

---

# 📊 Project Highlights

✔ Production-inspired architecture

✔ Mobile-first design

✔ Real-time GPS tracking

✔ JWT secured APIs

✔ SQLite database

✔ Tactical dashboard

✔ Live mapping

✔ Audio evidence recording

✔ Battery telemetry

✔ Nearby emergency services

✔ Rescue PIN protection

✔ Interactive monitoring

---

# 📷 Screenshots

> Replace these placeholders with your project screenshots.

## 📱 Mobile Application

```
assets/screenshots/login.png

assets/screenshots/home.png

assets/screenshots/sos.png

assets/screenshots/profile.png
```

Example:

```markdown
![Login](assets/screenshots/login.png)

![Home](assets/screenshots/home.png)

![SOS](assets/screenshots/sos.png)
```

---

## 🛰 Dashboard

```
assets/screenshots/dashboard.png

assets/screenshots/map.png
```

Example

```markdown
![Dashboard](assets/screenshots/dashboard.png)

![Map](assets/screenshots/map.png)
```

---

# 🎥 Demo

A demo video or GIF can greatly enhance the project showcase.

Example:

```markdown
## 🎥 Project Demo

![Demo](assets/demo/demo.gif)
```

or

```markdown
[Watch Demo Video](https://youtu.be/your-video-link)
```

---

# ⚡ Performance

- Fast Flask backend
- Lightweight SQLite database
- Low latency GPS updates
- Optimized Flutter UI
- Minimal API response time
- Efficient REST communication

---

# 🧪 Testing Checklist

Before deployment, verify the following:

- [ ] User Registration
- [ ] Login
- [ ] SOS Activation
- [ ] GPS Tracking
- [ ] Audio Recording
- [ ] Dashboard Updates
- [ ] Rescue PIN
- [ ] SOS Deactivation
- [ ] Nearby Hospital Detection
- [ ] Nearby Police Detection
- [ ] Battery Updates
- [ ] API Connectivity

---

# ❓ Troubleshooting

## Database Error

```
sqlite3.OperationalError:
no such column
```

Delete

```
instance/emergency_system.db
```

Restart the backend.

---

## Flutter Cannot Connect

Check that:

- Flask backend is running
- Ngrok tunnel is active
- `baseUrl` matches the current Ngrok URL
- Internet connection is available

---

## GPS Not Updating

Verify that:

- GPS is enabled
- Location permissions are granted
- Internet connection is active

---

## Authentication Issues

If JWT errors occur:

- Login again
- Clear app storage
- Restart backend

---

## Common Flutter Commands

```bash
flutter doctor

flutter clean

flutter pub get

flutter run
```

---

# 💡 Best Practices

- Keep the backend running before launching Flutter.
- Always update the Ngrok URL after restarting the tunnel.
- Test GPS outdoors for better accuracy.
- Regularly back up the SQLite database.
- Change the default Rescue PIN before production use.

---
# 🛣 Roadmap

Guardian Elite is continuously evolving. Planned enhancements include:

## Artificial Intelligence

- [ ] AI Threat Detection
- [ ] AI Incident Classification
- [ ] Suspicious Activity Recognition
- [ ] Emergency Severity Prediction

---

## Mobile Features

- [ ] Voice Activated SOS
- [ ] Shake Phone to Trigger SOS
- [ ] WearOS Support
- [ ] Apple Watch Support
- [ ] Offline SMS Emergency Alerts
- [ ] Live Video Streaming
- [ ] Background Crash Detection

---

## Dashboard Improvements

- [ ] Multi-User Monitoring
- [ ] Incident Replay
- [ ] Heatmaps
- [ ] Dark Mode
- [ ] Analytics Dashboard
- [ ] Export Incident Reports (PDF)

---

## Cloud Features

- [ ] PostgreSQL Support
- [ ] Docker Deployment
- [ ] Firebase Cloud Messaging
- [ ] AWS Deployment
- [ ] Azure Deployment
- [ ] Kubernetes Support

---

# 💼 Use Cases

Guardian Elite can be used in numerous real-world scenarios:

- 👩 Women's Safety
- 🎓 College & Campus Security
- 🚖 Cab & Ride Safety
- 🧗 Solo Travelers
- 🚴 Adventure Sports
- 🏢 Employee Safety
- 🚑 Emergency Medical Response
- 👨‍👩‍👧 Family Tracking
- 👴 Elderly Care
- 🚨 Disaster Response

---

# 🎯 Why Guardian Elite?

Unlike a traditional SOS application, Guardian Elite provides **continuous situational awareness**.

Instead of sending only an emergency notification, the platform continuously shares valuable emergency intelligence including:

- 📍 Live GPS Coordinates
- 🎙 Audio Evidence
- 🔋 Device Battery Status
- 🛰 Movement History
- 🏥 Nearby Emergency Services
- 👮 Police Station Discovery
- 📡 Live Dashboard Monitoring
- 🔐 Secure Rescue PIN Authentication

The goal is to assist responders in making faster and better-informed decisions during emergencies.

---

# 🤝 Contributing

Contributions are welcome!

If you have ideas for improving Guardian Elite, feel free to contribute.

## Steps

### 1. Fork the repository

### 2. Create a feature branch

```bash
git checkout -b feature/AmazingFeature
```

### 3. Commit your changes

```bash
git commit -m "Added Amazing Feature"
```

### 4. Push your branch

```bash
git push origin feature/AmazingFeature
```

### 5. Open a Pull Request

Every contribution—whether it's fixing a bug, improving documentation, or adding a feature—is appreciated.

---

# 📜 License

This project is licensed under the **MIT License**.

You are free to:

- Use
- Modify
- Distribute
- Fork

Please include the original license when redistributing the project.

---

# 🙏 Acknowledgements

Special thanks to the open-source technologies that made this project possible.

- Flutter
- Flask
- Python
- SQLite
- Leaflet.js
- OpenStreetMap
- Overpass API
- JWT
- Ngrok

---

# 👨‍💻 Author

## Krishna Chandra Panda

**Bachelor of Computer Applications (BCA)**

Passionate about building secure, scalable, and impactful software solutions in the domains of:

- Emergency Response Systems
- Artificial Intelligence
- Cybersecurity
- Full Stack Development
- Mobile Application Development

### 📍 Location

Bangalore, Karnataka, India

---

### 📧 Email

**Krishnachandra9877@gmail.com**

---

### 💼 LinkedIn

https://www.linkedin.com/in/krishnachandra16/

---

### 💻 GitHub

https://github.com/krishnachandra-16

---

# ⭐ Support the Project

If you found this project useful or interesting:

⭐ Star this repository

🍴 Fork the project

🐛 Report bugs

💡 Suggest new features

📢 Share it with others

Your support motivates future development!

---

# 📊 Repository Stats

Once the repository is public, you can enhance this section by adding dynamic GitHub badges such as:

- Repository Stars
- Fork Count
- Open Issues
- Contributors
- Last Commit
- GitHub Actions Build Status

These badges provide visitors with an instant overview of the project's activity and health.

---

# 🚀 Final Thoughts

Guardian Elite was built with a simple vision:

> **Technology should empower people and help save lives when every second matters.**

This project demonstrates how mobile development, backend engineering, geolocation, and real-time communication can be combined into a unified emergency response ecosystem.

Whether you're a developer, recruiter, or contributor, thank you for taking the time to explore Guardian Elite.

Every suggestion, contribution, or star helps make the project even better.

---

<div align="center">

# 🛡️ Guardian Elite

### Advanced Emergency Response & Tactical Command System

**Built with ❤️ by Krishna Chandra Panda**

*"Because every second counts."*

⭐ **If you enjoyed this project, don't forget to star the repository!** ⭐

</div>
