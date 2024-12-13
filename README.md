# UniversityPay - A Modern Fee Payment Solution
UniversityPay is a cutting-edge platform designed to simplify the fee payment process for university students. Built using the MERN stack (MongoDB, Express.js, React.js, Node.js), this application enhances the payment experience by integrating real-time notifications via Discord and secure payment processing through Razorpay.

# 🌟 Key Features
Streamlined Payments: Simplifies the fee payment process for students.
Instant Notifications: Provides updates directly through Discord.
Secure Payment Gateway: Razorpay integration ensures data and transaction safety.
Comprehensive Insights: Easily track and manage fee payment records.
# 🛑 System Requirements
Before setting up the project, ensure the following are installed:

- **Node.js**
- **npm** (bundled with Node.js)
- **MongoDB**

# 🛠️ Setup Instructions
Follow these steps to run the project locally:

1. Clone the Project
```bash
git clone https://github.com/SiriChandanaSykam/UniversityPay.git  
cd UniversityPay
```
2. Install Required Packages
```bash

# Install frontend dependencies  
cd frontend  
npm install  

# Install backend dependencies  
cd ../server  
npm install
```
3. Configure Environment Variables
Create a .env file inside the server directory and populate it with the following:

```env

SECRET_KEY=your_secret_key  
MONGO_URL=your_mongo_connection_string  

RAZORPAY_API_KEY=your_razorpay_api_key  
RAZORPAY_API_SECRET=your_razorpay_api_secret  

EMAIL=your_email  
EMAIL_PASS=your_email_password  

DISCORD_TOKEN=your_discord_bot_token  
ADMIN_CHANNEL_ID=your_admin_channel_id  
VERIFIED_CHANNEL_ID=your_verified_channel_id  
REJECTED_CHANNEL_ID=your_rejected_channel_id
```
Replace the placeholders with your actual credentials.

🚀 Running the Application
Frontend
Start the React application from the frontend directory:

```bash

cd frontend  
npm start
```
Access the app at http://localhost:3000. The app auto-reloads on file changes.

Backend
Run the Express server from the server directory:

```bash

cd server  
npm start
```
The backend will be available at http:/SiriChandanaSykam/localhost:8000.

# ⚡ Rate Limits and Expiration Policies
- **Local Storage Token Expiry:** 5 minutes (`frontend/Components/RollNumberForm.js`)
- **Bearer Token Expiry:** 5 minutes (`server/routes/feeRoute.js`)
- **API Rate Limit:** 40 requests per 15 minutes (`server/middlewares/validateInputMiddleware.js`)

## 🛠️ Technology Stack

### Frontend
- **React.js** - For building responsive user interfaces.

### Backend
- **Node.js** - JavaScript runtime for backend logic.
- **Express.js** - Framework for creating RESTful APIs.

### Database
- **MongoDB** - NoSQL database for data storage.

### Payment Integration
- **Razorpay** - Secure and efficient payment gateway.

### Notifications
- **Discord** - Used for real-time updates and admin alerts.

# 📄 License
This project is open-source and can be used or modified as needed.

