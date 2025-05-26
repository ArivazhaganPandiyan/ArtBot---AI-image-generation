 # ArtBot - AI Image Generator
 Turn your imagination into stunning visuals with ArtBot, a full-stack MERN application that transforms text prompts into AI-generated artwork using the Clipdrop API. Complete with secure authentication, credit management, and Stripe integration, ArtBot offers a seamless and user-friendly creative experience.

# 🌟 Features :

# ✨ Core Functionality
🔥 AI-Powered Image Generation (via Clipdrop API)

🔐 User Authentication with JWT (Register/Login)

🎟️ Credit System (5 free credits upon registration)

💳 Stripe Integration for purchasing additional credits

💾 Download Generated Images to your local system

# 🛠 Technical Highlights
🧱 MERN Stack – MongoDB, Express.js, React.js, Node.js

🛡 JWT Auth & Protected Routes – Secured with middleware

🔐 Password Hashing – Using bcrypt for secure storage

🌀 Framer Motion – For smooth UI animations

🎨 Tailwind CSS – Modern and responsive styling

🌍 Context API – Efficient global state management

# 🚀 Live Demo
Frontend: https://artbot-ai.netlify.app

Backend API: https://artbot-ai-image-generator.onrender.com

# 🏗️ Project Structure

artbot/
├── client/                  # React Frontend
│   ├── src/
│   │   ├── assets/          # Static assets
│   │   ├── components/      # Reusable components
│   │   ├── context/         # App state context
│   │   ├── pages/           # Page-level components
│   │   └── App.jsx          # Root React component
│
├── server/                  # Node.js + Express Backend
│   ├── controllers/         # Route logic
│   ├── middleware/          # JWT auth middleware
│   ├── models/              # Mongoose schemas
│   ├── routes/              # API routes
│   └── server.js            # Server entry point


# 🔧 Installation & Setup
#  Clone the Repository

git clone https://github.com/ArivazhaganPandiyan/artbot-ai-image-generation.git
cd artbot-ai-image-generation

#  Configure Environment Variables
server/.env
PORT=4000
MONGODB_URL="your_mongodb_connection_string"
JWT_SECRET="your_jwt_secret"
CLIPDROP_API="your_clipdrop_api_key"
STRIPE_SECRET_KEY="your_stripe_secret_key"

client/.env
VITE_BACKEND_URL="http://localhost:4000"

# Install Dependencies
# Backend
cd server
npm install

# Frontend
cd ../client
npm install

# Run the Application
# Run backend
cd server
npm run dev

# In another terminal, run frontend
cd ../client
npm run dev

# 📚 API Endpoints
# 🔐 Authentication

Endpoint	           Method	  Description

/api/user/register	 POST	    Register new user

/api/user/login      POST 	  Authenticate user

/api/user/profile	   GET	    Get logged-in user’s data (Protected)

# Image Generation

Endpoint	           Method	  Description

/api/image/generate	 POST	    Generate AI image from text input (Protected)

Request Body Example:
{
  "prompt": "A futuristic city skyline at sunset"
}

# 👤 User Management

Endpoint	           Method	  Description

/api/user/credits	   GET	    Retrieve user credit balance

# 🛒 Stripe Integration
📦 Multiple credit plans

🔐 Secure payment handling

🔄 Auto credit updates on success

🚨 Error handling with real-time notifications

# 🌈 Screenshots

# 🔐 Authentication 
![image](https://github.com/user-attachments/assets/1e2809d7-fc77-44cd-b29a-2b39a61884dd)
![image](https://github.com/user-attachments/assets/fe1092b5-1cd7-41a6-85b1-d08d434ba51d)
# 🏠 Homepage
![Screenshot 2025-05-23 165338](https://github.com/user-attachments/assets/6ac3e894-435d-4408-99cf-c64602c4b4b6)
# 🎨 Image Generation
![image](https://github.com/user-attachments/assets/6e3e1139-60fb-4ecb-a9f9-d31c51d85dc1)
# 💰 Credits Management
![image](https://github.com/user-attachments/assets/61b818bc-5f1a-4428-b3bb-1e433aca73e1)


# 📬 Contact
Arivazhagan Pandiyan
🔗 GitHub(https://github.com/arivazhagan-pandian)

