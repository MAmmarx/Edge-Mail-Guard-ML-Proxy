Edge Mail Guard - ML-Based Email Security Proxy

This project implements an asynchronous email proxy server with a machine learning-based spam detection system. It analyzes email metadata in real time to detect and block spam while allowing legitimate messages to pass through.

Machine Learning Email Filtering in Python

Overview
This project demonstrates how machine learning can be integrated with networking to build a real-time email security system. It uses a Random Forest classifier to analyze email metadata and classify messages as spam or legitimate traffic.

The system includes a modern graphical dashboard that displays live traffic logs, system status, and performance metrics.

Features
Asynchronous Email Proxy Server: Handles multiple client connections using asyncio
Machine Learning Spam Detection: Uses a Random Forest model for classification
Real-Time Email Analysis: Processes email headers before accepting messages
Live Monitoring Dashboard: Displays logs, system status, and traffic metrics
Attack Simulation: Simulates both spam and legitimate email traffic
Threaded Architecture: Keeps GUI responsive while running the server

How It Works
The server listens for incoming email connections using an asynchronous event loop
SMTP-like commands are processed to extract metadata from incoming messages
Only email headers are analyzed to reduce processing overhead
Features are extracted and passed to the trained machine learning model
The model classifies the message as spam or legitimate
Spam messages are blocked, while valid messages are accepted
The GUI updates in real time with logs and system statistics

Prerequisites
Python 3.x
Required libraries: tkinter, numpy, scikit-learn
