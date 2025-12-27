🏪 VendorStock – Smart Inventory Manager

VendorStock is a web-based smart inventory management system designed for small-scale vendors and shop owners.
It helps vendors track products, manage stock, record sales, analyze performance, and get AI-powered insights — all in one simple dashboard.

This project was built for a hackathon and fulfills the requirement of using Google Technologies.

🚀 Features
🔐 Authentication & User Management

Firebase Authentication (Email & Password)

Secure login & signup

Individual shop profiles for each vendor

📦 Inventory Management

Add, update, and delete products

Product categories (Grocery, Beverages, Snacks, etc.)

Real-time stock updates

Low-stock alerts

💰 Sales Management

Record daily sales

Automatic stock reduction

Profit calculation per sale

Daily sales & profit summary

📊 Analytics Dashboard

Total products & low-stock count

Category-wise inventory distribution

Inventory value overview

AI-generated recommendations

🤖 AI Assistant

Chat-based AI inventory assistant

Answers questions like:

“Which products are low in stock?”

“How can I increase profits?”

“Which category performs best?”

Context-aware responses using live inventory data

🛠️ Tech Stack
🌐 Frontend

HTML5

CSS3 (Responsive UI)

Vanilla JavaScript

Vite (for fast development & bundling)

☁️ Google Technologies Used

Firebase Authentication

Cloud Firestore (NoSQL Database)

Firebase Hosting

🤖 AI Integration

Cohere AI API (for chat assistant & analytics insights)

📁 Project Structure
VendorStock/
│
├── index.html          # Vite entry HTML file
├── src/
│   └── main.js         # Vite main JS file
│
├── dashboard.html      # Main application UI (auth + dashboard)
├── README.md           # Project documentation
└── vite.config.js      # Vite configuration

⚙️ Setup & Installation
1️⃣ Clone the Repository
git clone https://github.com/your-username/vendorstock.git
cd vendorstock

2️⃣ Install Dependencies (Vite)
npm install

3️⃣ Firebase Configuration

Create a Firebase project and enable:

Authentication → Email/Password

Firestore Database

Replace the placeholders in the script section:

const firebaseConfig = {
  apiKey: "_API_KEY",
  authDomain: "_AUTH_DOMAIN",
  projectId: "_PROJECT_ID",
  storageBucket: "_STORAGE_BUCKET",
  messagingSenderId: "_MESSAGING_SENDER_ID",
  appId: "_APP_ID"
};

4️⃣ Add Cohere API Key
const COHERE_API_KEY = "_COHERE_KEY";


⚠️ Never expose API keys in production.
For hackathons, this is acceptable.

▶️ Run the Project
npm run dev


Open browser at:

http://localhost:5173

🔐 Firestore Data Structure
Users Collection
users/
 └── userId
     ├── shopName
     ├── email
     ├── phoneNumber
     └── createdAt

Products Collection
products/
 └── productId
     ├── userId
     ├── name
     ├── category
     ├── costPrice
     ├── sellingPrice
     ├── quantity
     ├── lowStockThreshold
     └── createdAt

Sales Collection
sales/
 └── saleId
     ├── userId
     ├── productId
     ├── productName
     ├── quantitySold
     ├── totalAmount
     ├── profit
     └── saleDate

🎯 Problem Statement

Small vendors often rely on manual bookkeeping, leading to:

Stock mismanagement

Missed sales opportunities

Poor profit tracking

VendorStock solves this by providing a digital, intelligent, and easy-to-use inventory system accessible from any device.

✅ Solution Highlights

No technical knowledge required

Real-time updates using Firestore

AI-powered insights for smarter decisions

Mobile-friendly responsive UI

Secure & scalable cloud backend

🔮 Future Enhancements

Barcode scanning

Invoice & bill generation

Multi-shop management

Predictive demand forecasting

WhatsApp/SMS alerts

Progressive Web App (PWA)

🏆 Hackathon Readiness

✔ Uses Google Technology (Firebase)
✔ Solves real-world problem
✔ AI integration
✔ Scalable architecture
✔ Complete end-to-end product

👤 Author

Milind Garg, Poorvi Kulshrestha
Hackathon Project – VendorStock
