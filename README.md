Digital KYC Verification System
Introduction

This project presents a government-grade digital KYC (Know Your Customer) verification platform, designed for both web and mobile environments. It enables real-time identity authentication through document scanning, face matching, and liveness checks, wrapped in a professional government-style interface.

Core Highlights

Real-Time Capture: Instant camera-based document and face image collection

Multi-Language Support: Dynamic interface supporting six major Indian languages

Fake Detection: Simulated AI-based document authenticity verification

Cross-Platform Design: Fully responsive web app and React Native mobile app

Offline Compatibility: Mobile app can function without constant internet access

PDF Generation: Users can download or share verification reports instantly

Supported Identity Documents

Aadhaar Card

PAN Card

Driving License

Voter ID

Application Architecture
1. Web Platform (web-app/index.html)

Developed as a pure HTML5 standalone app — no frameworks used

Incorporates live video capture for ID and selfie verification

Simulates OCR and facial recognition processing using JavaScript

Implements fake document detection (20% random simulation rate)

Includes multi-language translation (English, Hindi, Telugu, Tamil, Bengali, Gujarati)

Features a responsive government-style interface with tricolor theme

Allows PDF report export and sharing

2. Mobile Platform (mobile-app/)

Built with React Native (v0.72.6) using Expo SDK 49

Utilizes expo-camera for real photo capture

Contains document and face recognition modules

Features a simple, formal UI suitable for government deployment

Works offline through local data handling

Technical Stack
Layer	Technology Used
Web	HTML5, CSS3, Vanilla JavaScript
Mobile	React Native + Expo
Camera APIs	MediaDevices (Web), expo-camera (Mobile)
Processing Simulation	TensorFlow.js references (mocked ML/AI behavior)
Styling	Indian government color palette (Saffron, White, Green)
Languages Supported	English (default), Hindi, Telugu, Tamil, Bengali, Gujarati
Project Directory Layout

KYC/
├── web-app/
│   ├── index.html           # Complete standalone browser app
│   └── webpack.config.js    # Web build configuration
├── mobile-app/
│   ├── App.js               # Main React Native entry point
│   ├── components/
│   │   ├── CameraScreen.js       # Camera functionality
│   │   └── DocumentProcessor.js  # Validation and analysis logic
│   ├── package.json         # Dependencies list
│   └── metro.config.js      # Metro bundler configuration
└── README.md


Setup Instructions
For Web

Open web-app/index.html in any modern browser.

Click “Start KYC Verification” to initiate the workflow.

Select a document type and capture the required images.

Follow the on-screen steps to complete verification.

For Mobile

Navigate to the mobile-app/ folder.

Run npm install to install all dependencies.

Launch with npx expo start.

Use Expo Go on your device or emulator to test the app.

Functional Overview
Key Features

Integrated camera access on both platforms

Live document and selfie capture

Simulated fraud detection and validation process

Full translation system with six-language support

Professional, emoji-free government design

Device-responsive and mobile-first layout

Detailed error handling and user guidance

On-demand PDF generation

Optional demo mode (phone verification bypass)

Offline-ready architecture for mobile

User Flow (Demo Simulation)

Welcome Screen → Launches KYC process (optionally skips OTP).

Document Type Selection → Choose Aadhaar, PAN, License, or Voter ID.

Capture Phase → Take photos of the document and face.

Verification Phase → System analyzes and validates inputs (simulated).

Results Screen → Displays success or failure with PDF download/share options.

Language Availability

English (default)

हिन्दी (Hindi)

తెలుగు (Telugu)

தமிழ் (Tamil)

বাংলা (Bengali)

ગુજરાતી (Gujarati)
