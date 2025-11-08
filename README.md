🏛️ KYC App – Digital Identity Verification Portal
📘 Overview

The KYC App is a government-grade digital identity verification system designed to streamline the Know Your Customer (KYC) process through secure and efficient document and face authentication.
It features both web and mobile applications, supporting real-time document scanning, face verification, and simulated AI-based validation, presented in a professional Indian government-style interface.

🚀 Key Features

Multi-Platform Support – Fully functional web and mobile applications

Real-Time Capture – Live document and selfie image acquisition via camera

Face Verification – Liveness and match detection (simulated)

Document Validation – Fake document detection simulation (20% random rate)

Multi-Language Interface – English, Hindi, Telugu, Tamil, Bengali, Gujarati

PDF Report Generation – Download or share verification summaries

Offline Functionality – Mobile version supports offline KYC flow

Government-Style UI – Clean, emoji-free interface with tricolor palette

Error Handling – Detailed feedback for incomplete or invalid data

🧩 Supported Documents

Aadhaar Card

PAN Card

Driving License

Voter ID

🖥️ Web Application (web-app/)
Features

Pure HTML5/CSS3/JavaScript (no frameworks)

Live Camera Integration via MediaDevices.getUserMedia()

OCR & Face Processing Simulation using TensorFlow.js references

Multi-Language Translation and dynamic UI updates

Mobile-Responsive Layout compatible across all devices

PDF Report Generation for verification results

Running the Web App

Open web-app/index.html in any modern browser

Click “Start KYC Verification”

Select a document type and capture images

Complete verification and download the report

📱 Mobile Application (mobile-app/)
Features

Built with React Native (v0.72.6) and Expo SDK 49

Uses expo-camera for real photo and video capture

Contains DocumentProcessor and CameraScreen components

Fully offline-capable with local data handling

Consistent government-style UI

Running the Mobile App

Navigate to the mobile-app/ directory

Install dependencies:

npm install


Start the Expo development server:

npx expo start


Scan the QR code with the Expo Go app or run on an emulator

⚙️ Technical Stack
Component	Technology
Web	HTML5, CSS3, JavaScript
Mobile	React Native (Expo SDK 49)
Camera Access	MediaDevices API (Web), expo-camera (Mobile)
Processing	Simulated AI/ML via TensorFlow.js references
Styling	Government color scheme – Saffron, White, Green
Languages Supported	English, Hindi, Telugu, Tamil, Bengali, Gujarati
📁 Project Structure
KYC/
├── web-app/
│   ├── index.html           # Complete standalone web application
│   └── webpack.config.js    # Build configuration
├── mobile-app/
│   ├── App.js               # Main React Native entry point
│   ├── components/
│   │   ├── CameraScreen.js       # Camera functionality
│   │   └── DocumentProcessor.js  # Document validation logic
│   ├── package.json         # Dependencies
│   └── metro.config.js      # Metro bundler configuration
└── README.md

🔄 Demo Workflow

Welcome Screen → Start KYC (optional OTP bypass)

Select Document Type → Choose Aadhaar, PAN, License, or Voter ID

Capture Stage → Take photo of document and face

Verification Stage → AI-based analysis (simulated)

Result Stage → Display validation status and allow PDF download/share

🌐 Language Options

English (default)

हिन्दी (Hindi)

తెలుగు (Telugu)

தமிழ் (Tamil)

বাংলা (Bengali)

ગુજરાતી (Gujarati)

🧠 Future Enhancements

Integration with actual OCR/Face Recognition APIs

Secure backend with encrypted document storage

Biometric verification via government APIs

Cloud-based analytics for fraud detection
