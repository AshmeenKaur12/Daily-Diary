# Day 23 — Face Recognition-Based Attendance System

**Date:** July 23, 2025

---

## Project Summary

On Day 23, I finalized and tested the **Face Recognition Attendance System** using **Python**, **OpenCV**, and the **face_recognition** library.

This system identifies individuals via webcam and logs their attendance in a `.csv` file. It uses 128-dimensional facial embeddings for accurate real-time recognition, with instant user feedback and clear UI distinctions between known and unknown faces.

---

## Features

### Encoding of Known Faces
- Images stored in `dataset/` (e.g., `john.jpg`, `emma.png`)
- Encoded using `face_recognition` into 128-d vectors
- Only one-time encoding required at startup

### Real-Time Recognition
- Activates webcam using OpenCV
- Detects faces in live frames and compares with known encodings
- Displays:
  - Green box with name for **recognized** individuals
  - Red box with "Unknown" label for **unrecognized** faces

### Attendance Logging
- Logs name and current timestamp to a `.csv` file
- Avoids duplicate entries during the same session
- Example:
  ```csv
  Name,Time
  Emma,2025-07-23 09:10:21
  ```
  
---

## User Feedback

- **Encoding**: Shows `"Encoding known faces..."` and `"Encoding complete."`
- **Logging**: Prints names and timestamps when attendance is marked
- **Duplicate Check**: `"JOHN is already marked."`
- **Unknown Handling**: `"Unknown face detected. Not marking attendance."`
- **Exit**: Clean shutdown on pressing `q`

---

## System Performance

- **Speed**: Near real-time recognition with low latency
- **Accuracy**: High for well-lit, frontal faces

### Limitations

- Poor performance in low light or with partial/angled faces  
- Cannot differentiate between identical twins  
- Accuracy depends on quality of dataset images  

---

## Scalability

To add a new person:

- Just place a labeled image in the `dataset/` folder  
- No code changes needed  
- System will automatically encode and include the new face on the next run

---

**By:** Ashmeen Kaur  
**URN:** 2302486  
**CRN:** 2315030

---

> *"Technology that sees, recognizes, and remembers — welcome to intelligent attendance."*
