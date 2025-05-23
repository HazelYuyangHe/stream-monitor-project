# Streaming Performance Monitor (Iter 3)

This project is part of Iteration 3 for our CS 5700 course. Our objective was to monitor key video streaming performance metrics in real time — including latency, frame loss, and bitrate fluctuations — using a browser-based solution built with HLS.js and standard HTML/JavaScript.

---

## 💡 User Story

- 👤 Who: As a network engineer  
- 📈 What: I want to monitor latency, frame loss, and bitrate fluctuations in real time  
- 🎯 Why: So that I can identify network issues and improve streaming performance  

---

## 📁 Project Overview

We created a lightweight HTML/JS-based tool that:

- Loads a live HLS test stream  
- Monitors key performance metrics from the browser  
- Requires no installation — runs in any modern browser  

📊 The real-time metrics displayed include:

- Bitrate Estimate (from hls.js)
- Dropped Frames
- Total Frames Played
- Realistic latency approximation using buffered.end(0) - currentTime  

---

## 🔧 How to Use

1. Download or clone this repository  
2. Open the file index.html in Chrome, Firefox, or any modern browser  
3. Observe the live stats panel below the video  
4. Use Chrome DevTools → Network → Throttle → select a slower network (e.g., 3G)  
5. Watch how bitrate, latency, and dropped frames change dynamically

---

## 🎬 Demo

We recorded a demonstration showing how the system reacts to changing network conditions, including:

- Real-time drops in bitrate under 3G/4G throttling  
- Increased frame loss under poor connections  
- Changes in latency calculated from playback buffering

📺 Demo video link:  
- https://www.youtube.com/watch?v=adcJLp3uoOU (3G)
- https://www.youtube.com/watch?v=izYiyJgkU9c (4G Slow)
- https://www.youtube.com/watch?v=6ITSGXRJVnk (4G Fast) 


---

## 📘 Lessons Learned

- Buffered data in HTML5 video can be used to approximate latency effectively
- HLS.js provides access to real-time bandwidth estimation with minimal setup
- Simulating poor networks using DevTools allows reliable test scenarios
- Logging and visualizing metric changes enhances understanding of streaming reliability

---

## 👥 Team Contributions

| Member        | Contribution                                                                     |
|---------------|----------------------------------------------------------------------------------|
| Yuyang He     | Built front-end UI, integrated HLS.js, and implemented real-time metric display logic |
| Yachen Wang   | Conducted network simulation tests, analyzed bitrate/frame drop variations under throttling |
| Ningxi Yang   | Wrote report content, created video demo, and documented findings in README.md |

---

## ✅ Tech Stack

- HTML / CSS / JavaScript  
- HLS.js (via CDN)  
- Chrome DevTools (for throttling simulation)  
- QuickTime / OBS (for demo recording)

---

## 📂 File Structure

- index.html — Main web app with HLS player and performance monitor  
- README.md — This file  

