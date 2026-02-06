# 🛡️ Project SafeFlow: Industrial Digital Twin & HMI
> **A High-Performance IT/OT Converged Simulation for Critical Infrastructure Security.**



## 🌐 Overview
Project SafeFlow is a professional-grade **Digital Twin** of an industrial high-pressure valve system. Developed to bridge the gap between **Software Engineering (IT)** and **Operational Technology (OT)**, this project demonstrates how modern web technologies (React/Vite) can interface with industrial logic and cybersecurity monitoring to prevent catastrophic equipment failure.

Targeted at the high-stakes industries of **Aerospace, Pharmaceuticals, and Utilities**, SafeFlow simulates a real-world Human-Machine Interface (HMI) built to **ISA-101 standards**.

---

## 🏗️ System Architecture
The project is built on a three-tier "Bulletproof" architecture:

1. **The Digital Twin (The Logic):** A physics-based React model simulating real-time Pressure (PSI) and Flow (L/min) variables.
2. **The HMI Layer (The Interface):** A high-performance, gray-scale dashboard designed for 12-hour operator shifts, focusing on "Clarity at a Glance."
3. **The Watchdog (The Security):** A background **Bash/PowerShell** script that audits the system logs to detect unauthorized access or AI-driven "spoofing" attacks.



---

## ✨ Key Features

### 🔧 Industrial Logic & Interlocks
The valve is protected by a **Safety Interlock Array**. It will not open unless a specific sequence is met:
* **Pre-condition:** Vent Fan must be `ACTIVE`.
* **Stability:** Pressure must be below `150 PSI`.
* **Authorization:** Sequential bypass codes must be entered in order.

### 🎭 Visual States
* **The Victory Dance:** A rhythmic, pleasing flicker and firing of bulbs/indicators upon successful completion of the safety sequence.
* **The Haunting (Security Breach):** An ominous, high-frequency flickering state triggered by safety violations or "Impossible" interactions (simulated cyber-attack).

### 🛡️ Cybersecurity Monitoring
Includes a background script that performs:
* **Log Auditing:** Monitors `activity.log` for anomalous patterns.
* **Hardening:** Simulates a hardware lockdown if a breach is detected.

---

## 🛠️ Tech Stack

| Category | Technology | Industry Relevance |
| :--- | :--- | :--- |
| **Frontend** | React 19, Vite | Modern HMI/SCADA Systems |
| **Styling** | Tailwind CSS, Framer Motion | High-Performance UI/UX |
| **Scripting** | Bash (Linux) / PowerShell | OT Security & System Hardening |
| **Logic** | Custom React Hooks | Digital Twin & Process Control |
| **Compliance**| ISA-101, IEC 62443 | Industrial Safety Standards |

---

## 🚀 Getting Started

### 1. Installation
```bash
# Clone the repository
git clone [https://github.com/](https://github.com/)[YOUR_GITHUB_USERNAME]/[PROJECT_NAME].git

# Navigate to the project
cd [PROJECT_NAME]

# Install dependencies
npm install

# Run the HMI
npm run dev
