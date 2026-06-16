OVERVIEW

FAHAD (Deepfake Image Verification Application) is an offline, AI-powered mobile application designed to detect AI-generated and manipulated images (deepfakes). The application uses a locally deployed Vision Transformer (ViT) model converted to TensorFlow Lite (TFLite) to perform image verification directly on the user's device without requiring an internet connection.

The system aims to address the growing problem of digital misinformation and privacy concerns associated with cloud-based verification tools by providing a secure, fast, and privacy-preserving solution.

OBJECTIVES
- Detect AI-generated and manipulated images offline.
Protect user privacy by processing all images locally.
Generate credibility scores and detailed verification reports.
Store verification history locally for future reference.
Provide an accessible verification tool even in low-connectivity environments.
Features
Offline Image Verification
Upload and verify images without an internet connection.
Supports:
JPG (.jpg)
JPEG (.jpeg)
PNG (.png)

AI-Powered Detection
Utilizes a Vision Transformer (ViT) model.
Performs on-device inference using TensorFlow Lite.
Generates:
Credibility Score (%)
Classification Result (Authentic / Manipulated)
📄 Detailed Verification Report

Displays:

Credibility score
Classification result
Verification date and time
Metadata information (if available)
AI analysis summary
📚 Verification History
Stores previous verification results locally using SQLite.
Allows users to review past reports through an interactive dashboard.
Privacy-First Architecture
Fully offline operation.
No image uploads to external servers.
No cloud dependency.
All data remains on the user's device.
System Architecture

User Interface (Flutter)
↓
Application Logic
↓
Image Preprocessing
↓
Vision Transformer (TensorFlow Lite)
↓
Verification Result Generation
↓
SQLite Local Database
