# BiblioFlow - Library Management System

A modern, enterprise-grade Library Management System built with React, Node.js, and MySQL.

## Features
- **Dynamic Hierarchy Control**: Manage Library -> Section -> Shelf -> Category -> Book Format with strict rule validation.
- **Modern Dashboard**: KPI cards, real-time charts, and recent activity monitoring.
- **Premium UI**: Glassmorphism, smooth animations, and tailored color palettes.
- **Secure**: JWT-based authentication and role-based access control.

## Tech Stack
- **Frontend**: React, Tailwind CSS, Recharts, Framer Motion, Lucide Icons.
- **Backend**: Node.js, Express, JWT, MySQL.

## Setup Instructions

### 1. Database Setup
1. Open your MySQL client (e.g., MySQL Workbench, XAMPP, or Terminal).
2. Execute the SQL commands found in `server/schema.sql`.
   - This will create the `library_system` database and necessary tables.
   - It also seeds a default admin user.

### 2. Environment Configuration
Check `server/.env` and update the database credentials if necessary:
```env
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_password
DB_NAME=library_system
JWT_SECRET=supersecretkeylibrary
```

### 3. Install Dependencies
Run the following in the root directory:
```bash
# In server directory
cd server && npm install

# In client directory
cd client && npm install
```

### 4. Start the Application
You can use the provided PowerShell script:
```powershell
./start-app.ps1
```
Or run them manually in two separate terminals:
**Terminal 1 (Backend):**
```bash
cd server && npm run dev
```
**Terminal 2 (Frontend):**
```bash
cd client && npm run dev
```

## Login Credentials
- **Username**: `admin`
- **Password**: `password123`
