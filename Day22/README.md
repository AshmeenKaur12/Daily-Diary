# Day 22 — Face Recognition Attendance System (Improved with CSV Logging)

**Date:** July 22, 2025

---

## Project Overview

This project implements a **Face Recognition-Based Attendance System** using **OpenCV**, **face_recognition**, and **Pandas** in Python.  
It captures live video from a webcam, detects and recognizes known faces from a dataset, and logs attendance in a timestamped CSV file.

---

## System Workflow

1. **Load Known Faces**  
   - Reads images from the `dataset/` folder  
   - Extracts names and computes 128-d face encodings

2. **Start Webcam Feed**  
   - Uses OpenCV to start live video

3. **Frame Preprocessing**  
   - Resize frame for performance  
   - Convert from BGR (OpenCV) to RGB (face_recognition)

4. **Face Detection and Encoding**  
   - Detects face locations  
   - Encodes current faces

5. **Face Matching**  
   - Compares detected encodings with known encodings  
   - Picks the closest match using Euclidean distance

6. **Mark Attendance**  
   - If recognized and not already marked, log name and time  
   - Writes to a CSV file like `attendance_2025-07-22_10-35-41.csv`

7. **Display Output**  
   - Shows webcam window with name overlay and bounding boxes  
   - Green = known, Red = unknown

---

**By:** Ashmeen Kaur  
**URN:** 2302486  
**CRN:** 2315030

---

> *"Technology that sees, recognizes, and remembers — welcome to intelligent attendance."*
