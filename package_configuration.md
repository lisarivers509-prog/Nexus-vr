{
"name": "nexusvr-remote",
"version": "1.0.0",
"description": "Ultra-Low Latency WebVR Remote Desktop Hub optimized for Standalone VR Headsets and Low-End Hardware",
"main": "www/index.html",
"scripts": {
"build": "npx cap copy android",
"open:android": "npx cap open android",
"sync": "npx cap sync android"
},
"keywords": \[
"vr",
"webvr",
"webxr",
"virtual-desktop",
"remote-desktop",
"webrtc",
"apk",
"quest",
"pico"
\],
"author": "NexusVR Team",
"license": "MIT",
"dependencies": {
"@capacitor/android": "^5.7.0",
"@capacitor/cli": "^5.7.0",
"@capacitor/core": "^5.7.0"
}
}
