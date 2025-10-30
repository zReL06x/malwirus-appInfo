# Malwirus – Privacy Policy

This repository hosts the public Privacy Policy for the Malwirus Android application.

## App Privacy Summary
- **No data collection**. Malwirus does not collect, transmit, or store personal data on external servers.
- **On-device processing**. SMS scanning, URL extraction, and device security checks happen locally on your device.
- **URL checks via Google Safe Browsing**. When you scan a link, only that URL is sent to the Google Safe Browsing API to verify potential risks. No personal identifiers are attached by Malwirus.
- **No analytics or ads identifiers**. The app does not use analytics tracking or advertising identifiers.

## Permissions and Purpose
- **SMS read/receive**: detect suspicious messages and extract URLs for local analysis.
- **Internet and network state**: query Google Safe Browsing for URLs you choose to scan.
- **Notifications and foreground service**: provide real-time alerts about potential threats.
- **Screen capture/record detection and device state signals**: warn you about risky device conditions.

## Data Retention
- Malwirus retains no personal data on external servers.
- Local scan history remains on your device and can be cleared in-app at any time.

## Third-Party Services
- **Google Safe Browsing API** is used solely to check if a scanned URL may be unsafe. Google may process the URL under its own terms and privacy policy.

## Children’s Privacy
- Malwirus is not directed to children under 13 and does not knowingly collect personal information from children.

## Changes and Contact
- This policy may be updated to reflect improvements or legal requirements. Updates are posted on the policy page.
- For questions, use the developer contact provided on the app store listing.

---

# Android Malwirus Security Application

## Overview
Android Malwirus is a comprehensive security application designed to protect Android devices from various security threats. The application implements multiple security features including SMS protection, web security, and device security monitoring.

## Features

### 1. SMS Security
- SMS monitoring and filtering using machine learning classification
- Protection against malicious SMS messages with confidence scoring
- Automatic detection and scanning of URLs in SMS messages
- Whitelist management for trusted phone numbers (limited to 11 digits)
- SMS history tracking with detailed threat information
- Centralized notification system for security alerts

### 2. Web Security
- Web browsing protection using Google SafeBrowsing API
- Malicious website detection in SMS messages
- Configurable URL scanning with toggle option in settings
- Detailed history of scanned URLs with threat information

### 3. Device Security
- Device security monitoring dashboard
- Screen capture detection
- Screen recording detection
- Root/jailbreak detection
- Security status reporting with actionable insights
- Real-time device security assessment

### 4. Additional Security Features
- Real-time security monitoring
- Security history tracking with detailed threat information
- Customizable security settings
- Background and foreground services for continuous protection
- Android 14 (API 34) compatibility with proper background execution restrictions
- Adaptive notifications based on detected threats

## Technical Details

### Requirements
- Android SDK 27 (Android 8.1) or higher
- Target SDK 34 (Android 14)
- Internet connectivity for URL scanning
- SMS permissions
- Foreground service permissions
- Screen capture/recording detection permissions

### Key Components
- `SplashArt`: Initial launch screen
- `MainActivity`: Main application interface
- `SMS_Activity`: SMS management interface
- `WebSecurity`: Web browsing protection features
- `DeviceSecurity_Activity`: Device security monitoring dashboard
- `Settings_Activity`: Application settings management
- `History_Activity`: Enhanced security history viewing with detailed threat information
- `SmsReceiver`: Background SMS monitoring service
- `SpamOptionsService`: Foreground service for handling security interactions
- `SafeBrowsingService`: URL scanning service using Google SafeBrowsing API

### Security Features
- Talsec Security integration for enhanced protection
- ONNX runtime for machine learning spam detection
- Real-time threat detection and notification
- Background service monitoring with foreground service capabilities
- Adaptive notification system based on threat severity and user settings
- URL scanning with configurable settings

## Permissions Required
- Internet access
- Network state access
- SMS reading and receiving
- Screen capture/recording detection
- Foreground service
- Package installation
- Notifications
- Receiver boot completed (for starting services on device boot)

## Development
The application is built using:
- Kotlin/Java
- AndroidX libraries
- Material Design components
- ONNX runtime for ML capabilities
- Google SafeBrowsing API for URL scanning
- Talsec Security SDK
- Coroutines for asynchronous operations
- Foreground services for Android 14 compatibility

## Security Considerations
- The application implements multiple layers of security
- Uses modern Android security best practices including foreground services
- Implements background monitoring with proper Android 14 compatibility
- Provides user control over security features through configurable settings
- Maintains detailed security history for audit purposes
- Centralized notification system to prevent duplicate alerts

## Recent Updates
- Enhanced URL scanning with configurable options
- Improved notification system to prevent duplicate alerts
- Added foreground service support for Android 14 compatibility
- Centralized SMS processing to improve efficiency
- Enhanced history display with detailed threat information
- Added phone number input validation in whitelist management
- Optimized background processing for better battery performance

## Note
This application is designed for educational and research purposes to demonstrate Android security concepts and implementations. 