#  FaceCheck: Face Recognition-Based Study Room Reservation System

###  Project Overview
**FaceCheck** is a computer vision-based study room check-in system built to modernize how students reserve and access rooms at Arizona State University. The system uses **real-time facial recognition** to provide secure, contactless authentication—replacing outdated, manual methods like email logins or ID swipes.

Designed for speed, usability, and deployment-readiness, this system aims to reduce no-shows and misuse of university resources.

---

###  Project Objective
To develop a lightweight, efficient, and privacy-conscious solution for **automated study room check-ins**, using face recognition to log student access securely and in real time.

---

###  Problem Statement
Manual room reservation systems (email logins, ID cards) are slow, error-prone, and often misused. This leads to:
- Long queues or delays
- Unfair usage
- Increased no-show rates

There’s a need for a fast, secure, and **touchless** alternative that works seamlessly in academic environments.

---

###  Solution Highlights
- 🔓 **Face recognition-based check-in** via webcam
- 🔁 Real-time matching against stored face encodings
- ✅ On match → access granted, booking logged
- ❌ On failure → access blocked, retry option
- 🧩 Flask-based backend for processing and file-based logging
- 🖥️ Local deployment (cloud-compatible)

---

###  Tech Stack

| Component              | Tool / Library                      |
|------------------------|--------------------------------------|
| Face Detection & Encoding | `face_recognition` (dlib + HOG + CNN) |
| Backend Web App        | `Flask`                             |
| Image Processing       | `OpenCV`                            |
| Frontend UI            | `Gradio` / HTML (optional)          |
| Deployment             | Localhost / Cloud-compatible        |
| Language               | Python                              |

---

###  Key Features
-  Touchless **face-based identity verification**
-  Near-instant check-in (<2s)
-  Booking log with timestamps
-  Easy new user registration
-  Adjustable matching threshold
-  Designed for real-world deployment at **ASU W. P. Carey**

---

###  Success Metrics
-  **95%+ accuracy** during local testing
-  **<2s check-in time**
-  **30% expected no-show reduction**
-  High simulated user satisfaction (pilot feedback)

---

### 🛡️ Privacy & Security
- 🧬 Only **face encodings**, not raw images, are stored
- 🔐 HTTPS-enabled communication (in production)
- ✅ GDPR-conscious design
- 🔮 Future: encrypted database, opt-in registration, audit trails

---

###  Validation & Testing
- Simulated various **lighting and angle conditions**
- Tuned threshold to **0.35** for better balance
- Realistic testing with webcam inputs
- Post-deployment plan includes:
  - Booking log audits
  - Error rate tracking
  - Real user feedback collection

---

###  Learnings
- Threshold tuning significantly improves recognition quality
- Lighting and face angle affect accuracy heavily
- Fallback UI is critical for handling edge cases
- Lightweight models offer speed but can be improved with deeper CNNs

---

###  Future Enhancements
-  Add **liveness detection** (blink, motion checks)
-  Mobile interface for remote face updates
-  Admin dashboard with analytics and usage insights
-  Group and multi-user bookings
-  Cloud deployment (Docker + AWS integration)
