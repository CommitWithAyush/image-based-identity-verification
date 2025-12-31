# Image-Based Identity Verification System

## 📌 Overview
This project is an image-based identity verification system designed to prevent impersonation and unauthorized profile image uploads in college ERP systems. The system verifies whether the uploaded profile image truly belongs to the logged-in student using facial recognition techniques.

In many existing ERP platforms, users can upload any image as a profile picture, which can lead to proxy attendance, identity misuse, and unauthorized benefits. This project adds a security layer by validating user identity before allowing profile image updates.

## ❗ Problem Statement
College ERP systems often lack identity verification while uploading profile images. As a result, students can upload images of other individuals, leading to impersonation and misuse of institutional services.

## 🎯 Objective
- To verify user identity using facial recognition
- To prevent unauthorized profile image uploads
- To reduce impersonation and proxy usage
- To enhance security in ERP systems
- To provide a scalable and integrable verification solution

## 💡 Proposed Solution
The system compares a reference image of a student with the newly uploaded image using face recognition. Facial features are extracted and converted into numerical embeddings, which are then compared to determine identity similarity.

If the similarity score crosses a predefined threshold, the upload is approved; otherwise, it is rejected.

## ⚙️ System Workflow
1. User logs into the ERP system
2. User uploads a profile image
3. System detects and extracts facial features
4. Face embeddings are generated
5. Uploaded image is compared with stored reference data
6. Similarity score is evaluated
7. Image upload is accepted or rejected accordingly

## 🏗️ Project Architecture
- Frontend: HTML, CSS
- Backend: Flask
- Face Recognition Module: Facial embedding generation and comparison
- Database: Stores user data and face encodings

## 🧰 Tech Stack Used

### Backend
- Python
- Flask

### Computer Vision & AI
- HOG (Histogram of Oriented Gradients) for feature extraction
- Face Recognition Library
- OpenCV

### Database
- SQLite / File-based storage

## ❓ Why This Tech Stack
- Python provides strong support for machine learning and computer vision
- Flask allows fast and lightweight backend development
- Face recognition libraries offer accurate pretrained models
- OpenCV efficiently handles image preprocessing

## 🔐 Security Features
- Prevents impersonation and proxy usage
- Ensures only genuine users can upload profile images
- Uses facial embeddings instead of raw images for comparison
- Rejects images with no face or multiple faces

## ⚠️ Challenges Faced
- Variations in lighting and facial expressions
- Low-quality images
- Selecting an optimal similarity threshold
- Handling multiple faces in one image

## 🚀 Future Enhancements
- Liveness detection to prevent photo/video spoofing
- Integration with attendance and examination systems
- Multi-factor authentication
- Cloud deployment for scalability
- Mobile application support

## 📂 Project Structure
```
image-based-identity-verification/
│
├── app.py
├── face_verification.py
├── database.py
├── templates/
├── static/
├── README.md
└── .gitignore
```

## 👨‍💻 Contributors
- Ayush Kumar Agarwal
- Deepak Bhatt

## 📄 License
This project is intended for academic and learning purposes.
