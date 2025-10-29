# 💬 BHARAT CONNECT - MERN Stack Real-Time Chat Application

### 🔗 [🚀 **Try It Live on Render**](https://bharatconnects-client.onrender.com/)

---

**BHARAT CONNECT** is a full-featured, real-time chat application built using the **MERN stack** (MongoDB, Express.js, React, Node.js) and **Socket.IO**.  
It provides users with a seamless and interactive chatting experience, including **real-time messaging**, **online status indicators**, **user authentication**, and **profile customization**.

---

## 🚀 Features

### 🔐 User Authentication
- Secure user registration and login system.  
- Passwords are encrypted using **bcryptjs** for enhanced security.  
- Authentication and sessions managed via **JSON Web Tokens (JWT)**.

---

### 💬 Real-Time Messaging
- Instant message delivery and reception between users using **Socket.IO (WebSockets)**.  
- Smooth and responsive chatting experience with no page reloads.

---

### 🔎 User Search
- Search for other registered users to start a new conversation.  

---

### 🟢 Online Status
- Green border indicator shows when a user is **online**, updated in real-time.

---

### 💬 Chat Management
- View a list of existing chats, sorted by **most recent messages**.  
- Click on a user to open the chat window and view conversation history.

---

### 📨 Message Features
- Send and receive **text messages** and **emojis**.  
- Upload and send **images** (stored securely using **Cloudinary**).  
- Display **message timestamps** (formatted as “Today”, “Yesterday”, or exact date).  
- Show **unread message count** for each chat.  
- Display **read receipts** with double-tick marks.

---

### 👤 User Profiles
- Users can **upload and update profile pictures**.  
- A dedicated **profile page** displays user info like **name**, **email**, and **account creation date**.

---

### 🎨 UI / UX
- Clean and modern interface built with **React**.  
- **Redux Toolkit** used for predictable and efficient global state management.  
- **Loading indicators** during API calls for better UX.  
- **Toast notifications** for real-time feedback (e.g., login success, errors).  

---

## 🧠 Tech Stack

### 🧩 Backend
- **Runtime:** Node.js  
- **Framework:** Express.js  
- **Database:** MongoDB (hosted on **MongoDB Atlas**)  
- **ODM:** Mongoose  
- **Real-Time Communication:** Socket.IO  
- **Authentication:** bcryptjs, jsonwebtoken  
- **Image Storage:** Cloudinary  
- **Development Tool:** Nodemon  

---

### 💻 Frontend
- **Library:** React  
- **State Management:** Redux Toolkit  
- **Routing:** React Router DOM  
- **HTTP Client:** Axios  
- **Real-Time Communication:** Socket.IO Client  
- **UI/UX:** HTML, CSS, React Hot Toast, Moment.js  

---

## 🧰 Tools
- **Package Manager:** npm  
- **API Testing:** Postman  

---

## 📁 Project Structure

The project is organized into two main folders for a clear separation of concerns:
BHARAT-CONNECT/
├── client/ # Contains all the Frontend React code
└── server/ # Contains all the Backend Node.js/Express code

---

## ⚙️ Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

---

### 🧾 Prerequisites

Before you begin, ensure you have the following installed:

- **Node.js** and **npm**
- A **MongoDB Atlas** account (for cloud database)
- A **Cloudinary** account (for image storage)
- **Postman** (optional) for testing APIs

---

## 🖥️ Backend Setup

### 1️⃣ Navigate to the Server Directory
```bash
cd server

2️⃣ Install Dependencies
npm install
3️⃣ Create an Environment File

Create a file named config.env in the root of the server directory.

4️⃣ Add Environment Variables

Insert your credentials and configurations in the file:
PORT_NUMBER=5000
CONN_STRING=mongodb+srv://<username>:<password>@cluster.mongodb.net/bharat-connect
SECRET_KEY=your_jwt_secret_key

CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
5️⃣ Start the Server
npm start


✅ The backend server should now be running at
👉 http://localhost:5000

💻 Frontend Setup
1️⃣ Navigate to the Client Directory
cd client

2️⃣ Install Dependencies
npm install

3️⃣ Configure Proxy

Ensure your package.json inside the client folder includes this line (to forward API requests to your backend):

"proxy": "http://localhost:5000"

4️⃣ Start the Client
npm start


✅ The React development server will now start automatically.
Open your browser and visit:
👉 http://localhost:3000




