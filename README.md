Freshness Detector 🍎
IoT + Computer Vision system to detect fruit freshness and verify expiry dates using ESP32-CAM and OCR — built for Flipkart GRiD 6.0 (Robotics Track)

Team Kanyarashi | Flipkart GRiD 6.0 — Robotics Track (via Unstop) | Oct 2024

An IoT + Computer Vision system that detects fruit freshness and verifies product expiry dates, aimed at reducing food spoilage losses across retail and supply chain operations.

Problem Statement

Roughly one-third of fruits become rotten before or during sale, causing significant economic losses across farmers, sellers, and food processing industries. Freshness and expiry checks are still largely manual — slow, inconsistent, and hard to scale. This project explores whether embedded hardware + computer vision can automate that check.

How It Works

The system combines two detection pipelines:

Freshness Classification — an image classification model (trained via Roboflow, compatible with TensorFlow/YOLO pipelines) identifies whether a fruit is fresh or spoiled from a captured image.
Expiry Date Verification (OCR) — an ESP32-CAM module captures an image of a product's printed label. The image is streamed to a lightweight web server hosted on the module, processed using Tesseract OCR to extract the manufacturing date, and compared against the current date to flag the product as valid or expired.
Grocery Item → ESP32-CAM Capture → Web Server (IP) → OCR Text Extraction
      → Date Parsing & Validation → Pass / Fail Result
Tech Stack
Category	Tools / Technologies
Firmware	C/C++, Arduino IDE, ESP32-CAM
Computer Vision	Roboflow, TensorFlow, YOLO
OCR	Tesseract OCR
Connectivity	WiFi, embedded web server
Hardware	ESP32-CAM module, sensor/camera interfacing
My Role

I led a 4-member team (Team Kanyarashi) from concept to working prototype — coordinating model training, firmware development, and OCR integration, and presenting the final solution at Flipkart GRiD 6.0 (Robotics Track).

Team:

Chethana Reddy Sanepalli — Team Lead
Mirthhulaa Surulivel Prasath
Venu Gopala Reddy Alla
Parnika Satish Surisetty

Gandhi Institute of Technology and Management (GITAM Hyderabad)
