# Video Streaming Using Cloud Computing on AWS

## 📌 Overview  
This project implements a **video streaming application** using **Amazon Web Services (AWS)** to provide **secure, scalable, and efficient** video hosting and streaming capabilities. Users can upload and view videos based on their role (guest or registered user).  

## 🚀 Features  
✅ **User Authentication** – AWS Cognito for user registration & login  
✅ **Secure Video Upload & Access** – AWS S3 for public/private video storage  
✅ **Role-Based Access Control (RBAC)** – Different access levels for guests and registered users  
✅ **REST API Backend** – Node.js-based backend for handling video uploads & retrieval  
✅ **Scalable Cloud Infrastructure** – AWS IAM, AWS S3, AWS Cognito  

## 🏗️ System Architecture  
The system consists of:  
- **Frontend**: HTML, CSS, JavaScript (User Interface)  
- **Backend**: Node.js (API server)  
- **Cloud Services**:  
  - AWS Cognito – User authentication & management  
  - AWS S3 – Secure video storage (public & private folders)  
  - AWS IAM – Role-based access control  

## 📜 Project Structure  
```
/cloud-video-streaming
│── backend/                      # Node.js Backend API
│   ├── routes/                   # API Routes (Auth, Upload, Retrieve)
│   ├── services/                 # AWS Integration (S3, Cognito)
│   ├── server.js                 # Main Server File
│── frontend/                     # Frontend UI (HTML, CSS, JavaScript)
│   ├── index.html                 # Homepage
│   ├── login.html                 # Login Page
│   ├── upload.html                # Video Upload Page
│── README.md                      # Project Documentation
│── package.json                    # Dependencies & Scripts
```

## 🛠️ Installation & Setup  

### 1️⃣ Prerequisites  
- **AWS Account** with IAM roles & S3 access  
- **Node.js** installed on your system  

### 2️⃣ Clone the Repository  
```bash
git clone https://github.com/Harshith422/cloud-video-streaming.git
cd cloud-video-streaming
```

### 3️⃣ Install Dependencies  
```bash
npm install
```

### 4️⃣ Configure AWS Credentials  
- Set up **IAM roles** with **S3 & Cognito access**  
- Update AWS credentials in `.env` file  
```env
AWS_ACCESS_KEY_ID=your_access_key
AWS_SECRET_ACCESS_KEY=your_secret_key
AWS_REGION=your_region
COGNITO_USER_POOL_ID=your_cognito_pool_id
S3_BUCKET_NAME=your_s3_bucket_name
```

### 5️⃣ Run the Backend Server  
```bash
node server.js
```

### 6️⃣ Open the Frontend  
- Open `index.html` in a browser  
- Users can **register, login, upload, and stream videos**  

## 🔍 API Endpoints  
| Method | Endpoint          | Description |
|--------|------------------|-------------|
| POST   | `/register`       | User registration |
| POST   | `/login`          | User login |
| POST   | `/uploadVideo`    | Upload a video (public/private) |
| GET    | `/getVideos`      | Retrieve video URLs |

## 🏁 Deployment  
- **Frontend:** Can be hosted on **S3, Netlify, or Vercel**  
- **Backend:** Can be deployed on **AWS Lambda, EC2, or Elastic Beanstalk**  

## 📌 Future Enhancements  
🔹 **Live Streaming Integration**  
🔹 **Video Processing & Transcoding**  
🔹 **AI-Based Content Recommendation**  
