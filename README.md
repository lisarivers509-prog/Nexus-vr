[nexusvr_readme.md](https://github.com/user-attachments/files/34347080/nexusvr_readme.md)
# 🪐 NexusVR — Next-Gen Remote VR & Desktop Sync

![NexusVR Banner](https://img.shields.io/badge/WebVR-Remote%20Desktop-00f0ff?style=for-the-badge&logo=virtualbox)
![License](https://img.shields.io/badge/License-MIT-7000ff?style=for-the-badge)
![Target Hardware](https://img.shields.io/badge/Hardware-Potato%20PC%20%2F%20Integrated%20GPU-emerald?style=for-the-badge)

**NexusVR** is an ultra-lightweight, single-file WebVR Remote Desktop hub designed to run seamlessly on low-spec "potato" PCs, integrated GPUs, and standalone VR headsets (Meta Quest, Pico, HTC Vive, PCVR). It enables low-latency desktop streaming, dynamic resolution downscaling, stereoscopic side-by-side (SBS) VR rendering, and direct WebXR headset pairing.

---

## ✨ Features & Capabilities

### 🥔 Potato PC Optimization Engine
* **Dynamic Resolution Downscaling:** Instantly switch between 0.5x Eco mode, 0.75x Balanced mode, and 1.0x Native scale to fit weak integrated GPUs.
* **FPS Frame Rate Target Capping:** Toggle between 30 FPS, 60 FPS, and 90 FPS to preserve host CPU/GPU cycles.
* **Low-Latency Hardware Codecs:** Hardware H.264 (AVC) encoding for fast decode on low-end hardware, with optional HEVC (H.265) and AV1 support.
* **Configurable Bitrate Limit:** Fine-tune stream bitrate from 1 Mbps (low Wi-Fi bandwidth) up to 100 Mbps (Ethernet).

### 🥽 Virtual Desktop & WebXR Compatibility
* **Stereoscopic SBS (Side-by-Side) Mode:** Native dual-lens rendering for mobile VR headsets, Google Cardboard, or standalone VR Web Browsers.
* **Interactive Geometry Controls:** Adjust screen curvature (0°–60°), virtual distance (1.0m–5.0m), and overall display scale.
* **In-VR Quick Connect Overlay:** Enter 6-digit VR PIN codes directly within the WebXR 3D space to pair standalone headsets without taking off the headgear.
* **Custom VR Environments:** Choose between *Void*, *Studio*, *Cyber Cinema*, and *Passthrough Grid* environments.

### 📊 Real-Time Stream Telemetry & System Diagnostics
* **System Diagnostic Benchmark:** Tests WebGL2 acceleration, WebXR API availability, GPU render-loop stability, WebRTC network latency, and video decoder capability.
* **Live Telemetry Dashboard:** Integrated Chart.js graphs displaying real-time stream FPS, decode/network latency (target `<15ms`), host CPU usage, and GPU encoder load.
* **6DOF Motion Controller Raycasting:** Emulate controller laser pointers and head-gyro orientation directly on the virtual desktop canvas.

---

## 🚀 Quick Start Guide

### Prerequisites
* Any modern web browser supporting HTML5 Canvas, WebGL2, and WebRTC (Chrome, Edge, Brave, Firefox, or Meta Quest Browser).
* No external server installation required for basic standalone emulation.

### Running Locally
1. Download or clone `index.html`.
2. Open `index.html` directly in your browser.
3. Click **"Run System Test"** in the top navigation bar to run an automatic diagnostic benchmark.
4. Click **"Apply Profile & Close"** to auto-apply optimal performance settings based on your hardware capabilities.

---

## 🎮 How to Connect a Standalone VR Headset (Meta Quest / Pico)

1. **Host PC:** Open NexusVR (`index.html`) on your host computer.
2. **VR Headset:** Open the VR browser on your headset (e.g., Meta Quest Browser) and navigate to the hosted NexusVR URL.
3. **Select Mode:** Click **"Headset SBS Mode"** or enter full-screen WebXR mode.
4. **Pair:** Note the 6-digit PIN code on your host display (e.g., `748-291`) and enter it using the In-VR keypad overlay.

---

## 🛠 Performance Presets Guide

| Mode | Res Scale | Target FPS | Bitrate | Recommended Hardware |
| :--- | :--- | :--- | :--- | :--- |
| **Potato PC Eco** | `0.5x` | 30 FPS | 4–8 Mbps | Intel HD Graphics / Older Laptops / 2.4GHz Wi-Fi |
| **Balanced** | `0.75x` | 30–60 FPS | 12–20 Mbps | Mid-tier Laptops / Integrated Vega / 5GHz Wi-Fi |
| **Ultra Native** | `1.0x` | 90 FPS | 50+ Mbps | Dedicated NVIDIA/AMD GPU / Wi-Fi 6 or Ethernet |

---

## 📜 Tech Stack

* **Frontend:** Single-file HTML5, CSS3, JavaScript (ES6+)
* **Styling:** Tailwind CSS (via CDN) + FontAwesome 6 Icons
* **Rendering Engine:** WebGL2 2D/3D Dual-Eye Stereo Canvas Pipeline
* **Telemetry & Analytics:** Chart.js
* **Networking Protocol:** WebRTC DataChannels & MediaStreams with AES-256 encryption

---

## 📄 License

Distributed under the MIT License. Feel free to modify and adapt for your own WebVR remote desktop setups!
