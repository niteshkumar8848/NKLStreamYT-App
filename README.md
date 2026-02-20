# NKLStream Android App

An Android application for NKLStreamYT - a synchronized watch party platform for watching YouTube videos together with friends in real-time.

**Web Version:** [NKLStreamYT](https://nklstreamyt.pages.dev)

---

## 📱 About This App

The NKLStream Android app brings the full watch party experience to your Android device. Join rooms, watch YouTube videos in perfect synchronization with friends, and enjoy peer-to-peer video/audio chat - all from your phone or tablet.

---

## ✨ Features

### Core Functionality
- 🎬 **Synchronized Playback** - Watch YouTube videos in sync with all room participants
- 🎙️ **Video/Audio Chat** - Peer-to-peer video calls with room members
- 💬 **Real-time Messaging** - Chat with friends during the watch party
- 🔐 **Room System** - Join rooms with secure 8-character codes

### User Experience
- 📱 **Mobile-Optimized** - Designed for Android phones and tablets
- 🎨 **Material Design** - Clean, modern Android UI
- ⚡ **Fast & Lightweight** - Only 1.5MB APK size

### Security
- 🛡️ **Secure Rooms** - 53.4 trillion possible room code combinations
- ✅ **Input Validation** - Protected against malicious inputs
- 🔒 **Encrypted Communication** - Secure WebRTC and Socket.IO connections

---

## 📦 Installation

### Prerequisites
- Android device running Android 5.0 (Lollipop) or higher
- Permission to install apps from "Unknown Sources" (if not from Play Store)

### Installation Methods

#### Method 1: Direct APK Installation
1. Download the `app-release-signed.apk` file
2. Open your file manager and navigate to the APK location
3. Tap on the APK to install
4. If prompted, allow "Install from unknown sources"
5. Follow the on-screen installation instructions
6. Once installed, tap "Open" to launch the app

#### Method 2: ADB Installation (For Developers)
```bash
# Connect your Android device via USB
adb install app-release-signed.apk
```

#### Method 3: Transfer & Install
1. Transfer the APK to your Android device (via USB, Bluetooth, cloud storage, etc.)
2. Open the file on your device
3. Follow the installation prompts

---

## 🚀 Getting Started

### First-Time Setup
1. Launch the app
2. Enter your display name (3-32 characters)
3. Grant camera and microphone permissions when prompted

### Creating a Room
1. Tap "Create Room" on the main screen
2. Share the 8-character room code with friends
3. Paste a YouTube URL and tap "Load Video"
4. Control playback for everyone in the room

### Joining a Room
1. Tap "Join Room" on the main screen
2. Enter the 8-character room code shared by the host
3. Wait for the host to load a video
4. Enjoy synchronized viewing!

---

## 🔧 Technical Details

| Specification | Details |
|---------------|---------|
| **Package Size** | ~1.5 MB |
| **Min Android Version** | Android 5.0 (API 21) |
| **Target Android Version** | Android 14 (API 34) |
| **Architecture** | ARM, ARM64, x86 |

### Permissions Required
- `INTERNET` - For connecting to rooms and streaming
- `CAMERA` - For video chat
- `MICROPHONE` - For voice chat
- `RECORD_AUDIO` - For audio chat (legacy)

---

## 🔗 Related Projects

### Main Web Application
- **Repository:** [NKLStreamYT](https://github.com/niteshkumar8848/NKLStreamYT)
- **Live Demo:** [nklstreamyt.pages.dev](https://nklstreamyt.pages.dev)

### Features (Web Version)
The Android app connects to the same backend as the web version, providing:
- Real-time synchronized YouTube playback
- WebRTC peer-to-peer video/audio calls
- Live chat messaging
- Room management with host controls

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────────┐
│                    Android App                          │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐     │
│  │   UI Layer  │  │  WebSocket  │  │   WebRTC    │     │
│  │  (Activities│  │  (Socket.IO)│  │   Client    │     │
│  │   & Views)  │  │             │  │             │     │
│  └─────────────┘  └──────┬──────┘  └──────┬──────┘     │
│                          │                 │            │
└──────────────────────────┼─────────────────┼────────────┘
                           │                 │
              ┌────────────┴──────┐  ┌──────┴───────┐
              │  Backend Server   │  │  P2P Peers   │
              │  (Socket.IO)      │  │  (WebRTC)    │
              └───────────────────┘  └──────────────┘
```

---

## ⚠️ Known Limitations

- **YouTube Only** - Works with YouTube video URLs
- **Max 4 Users/Room** - Limited by WebRTC mesh topology
- **Stable Internet Required** - Needs good connection for sync
- **Modern WebView** - Requires updated Android System WebView

---

## 📋 Version History

| Version | Date | Changes |
|---------|------|---------|
| v1.0 | Feb 2026 | Initial release with core features |

---

## 👨‍💻 About

**Developer:** Nitesh Kumar Lodh  
**Focus:** Real-time web applications, mobile development, WebRTC

### Connect
- 🔗 GitHub: [@niteshkumar8848](https://github.com/niteshkumar8848)
- 🌐 Web App: [nklstreamyt.pages.dev](https://nklstreamyt.pages.dev)

---

## 📜 License

This project is open source. All rights reserved.

---

<div align="center">
  <strong>✨ Watch together, anywhere ✨</strong>
</div>

