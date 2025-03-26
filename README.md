# Streaming Performance Monitor (Iter 3)

This project is part of Iteration 3 for our course. Our goal is to monitor key video streaming performance metrics: real-time latency, frame loss, and bitrate fluctuations.

## 💡 User Story

- 👤 Who: As a network engineer  
- 📈 What: I want to monitor latency, frame loss, and bitrate fluctuations in real-time  
- 🎯 Why: So that I can identify network issues and improve streaming performance  

## 📁 Project Contents

This project includes a lightweight HTML page that:

✅ Plays a live HLS test stream  
✅ Displays key streaming performance metrics every 2 seconds  
✅ Requires no installation – just open index.html in a browser  

The displayed metrics include:

- Bitrate Estimate (in kbps)
- Dropped Frames
- Total Frames Played
- Simulated Latency

## 🔧 How to Use

1. Download or clone this repository  
2. Open the file index.html in any modern browser (Chrome, Firefox, etc.)  
3. Watch the video and monitor performance in real time  
4. Use Chrome DevTools → Network → Throttle (e.g., Slow 3G) to simulate poor network conditions

## 🎬 Demo

A demo video recording can be found here:  
👉 [Demo Video Link](https://your-video-link-here.com)

## 📷 Screenshots

| Normal Network | Throttled Network |
|----------------|------------------|
| ![normal](screenshot-normal.png) | ![slow](screenshot-slow3g.png) |

## 📘 Lessons Learned

- We learned how to access playback performance data from browser APIs.
- We used HLS.js to extract bitrate estimates and frame data.
- We simulated different network conditions to evaluate the system.
- We better understood how network reliability directly affects streaming performance.

## 👥 Team Contributions

| Member        | Contribution                                                                     |
|---------------|----------------------------------------------------------------------------------|
| Yuyang He     | Frontend implementation (HTML/JS), HLS integration, performance display logic    |
| Yachen Wang   | Network simulation testing, screenshot capturing, performance comparison analysis|
| Ningxi Yang   | Report writing, video demo recording & editing, GitHub README documentation      |

## ✅ Tech Used

- HTML / JavaScript  
- HLS.js CDN  
- Chrome DevTools (Network Throttling)
