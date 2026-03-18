# Campus EventHub 🎓

Welcome to Campus EventHub—a premium, full-stack event management platform built specifically for universities and colleges. This system streamlines event discovery, registration, and administrative control with a stunning, modern user interface.

## 🌟 Key Features

### For Students
- **Interactive Dashboard:** Beautiful glassmorphic UI displaying upcoming events, active registrations, and personalized stats.
- **Seamless Registration:** One-click event registration with real-time status updates (Pending, Approved, Rejected).
- **Event Discovery:** Filter and search through technical, cultural, and sports events happening around campus.
- **Smart Analytics:** Track your participation and review events with an intuitive 5-star rating system.

### For Admins
- **Comprehensive Control Panel:** Visualize system health, event analytics, and registration trends through dynamic charts.
- **Event Management:** Create, update, and manage campus events with rich descriptions and category tagging.
- **User Management:** Super Admins can manage college admins and students, ensuring precise access control.
- **Registration Workflows:** Easily approve or reject student registrations directly from the dashboard.

## 🎨 Premium UI/UX Design
The frontend has been meticulously crafted with modern design principles:
- **Glassmorphism:** Elegant floating panels (`.glass-panel`) with frosted glass effects.
- **Dynamic Gradients:** Vibrant, mesh-gradient backgrounds that shift and interact.
- **Micro-Animations:** Fluid hover states, floating icons, and glowing shadows (`shadow-glow`) to make the interface feel alive.
- **Responsive Layout:** fully optimized for both desktop and mobile viewing with Tailwind CSS.

## 🛠️ Technology Stack

**Frontend:**
- React (Vite)
- Tailwind CSS v4 (with custom glowing utility system)
- React Router DOM
- Chart.js (Data Visualization)
- Lucide React (Icons)

**Backend:**
- Node.js / Express
- MongoDB (Mongoose)
- JWT Authentication

## 🚀 Local Setup Instructions

### Prerequisites
- Node.js (v18+)
- MongoDB Atlas account or local MongoDB server

### 1. Database Setup
Ensure you have a MongoDB connection string. Create a `.env` file in the `Backend` directory:
```env
PORT=4000
DB_CONNECT=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
FRONTEND_URL=http://localhost:5173
```

### 2. Run Backend
```bash
cd Backend
npm install
npm start
```

### 3. Run Frontend
```bash
cd frontend
npm install
npm run dev
```

Your frontend will be accessible at `http://localhost:5173`.

## 🛡️ Authentication & Authorization
The application uses secure JWT tokens stored in localStorage. Passwords are cryptographically hashed before hitting the database. Role-Based Access Control (RBAC) securely separates Student, College Admin, and Super Admin privileges.

## 🤝 Contribution
Contributions are welcome! If you're looking to add features or fix bugs, please fork the repository and submit a pull request.