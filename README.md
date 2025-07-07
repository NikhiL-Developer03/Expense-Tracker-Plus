# 💰 Expense Tracker Plus - Full-Stack MERN Application

A comprehensive expense tracking application built with the MERN stack (MongoDB, Express.js, React.js, Node.js) that helps users manage their finances with an intuitive interface and powerful features.

## 🌟 Overview

Build a Full-Stack MERN Expense Tracker that provides complete financial management capabilities with secure authentication, interactive dashboards, and comprehensive reporting features. This project demonstrates modern web development practices with React hooks, context API, styled-components, and RESTful APIs.

## ✨ Key Features

### 🔐 1. User Authentication
- **Secure Login & Sign-up** using JWT (JSON Web Tokens)
- Password encryption with bcrypt
- Protected routes and session management
- Automatic token refresh and logout functionality

### 📊 2. Dashboard Overview
- **Total Balance Display** - Real-time calculation of income minus expenses
- **Income Summary** - Total income with visual indicators
- **Expense Summary** - Total expenses with category breakdowns
- **Quick Stats Cards** - At-a-glance financial overview

### 💵 3. Income Management
- **Add Income Sources** - Multiple categories (Salary, Freelance, Investments, etc.)
- **View Income History** - Chronological list with dates and amounts
- **Delete Income Records** - Easy removal with confirmation
- **Export Income Data** - Download detailed reports in Excel format

### 💸 4. Expense Management
- **Add Expenses** - Categorized tracking (Food, Transport, Entertainment, etc.)
- **View Expense History** - Detailed expense timeline
- **Category-based Tracking** - Organize expenses by type
- **Delete Functionality** - Remove expenses with hover-to-reveal delete buttons
- **Export Expense Data** - Generate Excel reports

### 📈 5. Interactive Charts & Analytics
- **Bar Charts** - Monthly income vs expense comparison
- **Pie Charts** - Expense distribution by category
- **Line Charts** - Trend analysis over time
- **Visual Data Representation** - Easy-to-understand financial insights

### 🕒 6. Recent Transactions
- **Latest Records Display** - Quick access to recent income and expenses
- **Transaction History** - Complete chronological view
- **Real-time Updates** - Instant reflection of new transactions

### 📋 7. Comprehensive Reports
- **Excel Export** - Download complete income and expense data
- **Filtered Reports** - Generate reports by date range or category
- **Financial Summaries** - Detailed breakdown of financial activities

### 📱 8. Mobile Responsive Design
- **Cross-device Compatibility** - Works on desktops, tablets, and mobile devices
- **Responsive UI Components** - Adaptive layout for all screen sizes
- **Touch-friendly Interface** - Optimized for mobile interactions

### 🧭 9. Intuitive Navigation
- **Sidebar Menu** - Easy access to all features
- **Dashboard Navigation** - Quick links to Income, Expenses, and Reports
- **User-friendly Interface** - Clean and modern design
- **Logout Functionality** - Secure session termination

### 🗑️ 10. Smart Delete Functionality
- **Hover-to-reveal** - Delete buttons appear on hover over transaction cards
- **Confirmation Dialogs** - Prevent accidental deletions
- **Instant Updates** - Real-time removal from UI and database

## 🛠️ Tech Stack

### Frontend
- **React.js** - Component-based UI library
- **React Hooks** - useState, useEffect, useContext for state management
- **React Router** - Client-side routing and navigation
- **Styled Components** - CSS-in-JS styling solution
- **Chart.js & React-Chartjs-2** - Interactive data visualization
- **Axios** - HTTP client for API requests
- **React DatePicker** - Date selection component

### Backend
- **Node.js** - JavaScript runtime environment
- **Express.js** - Web application framework
- **MongoDB** - NoSQL database for data storage
- **Mongoose** - MongoDB object modeling
- **JWT** - JSON Web Tokens for authentication
- **bcrypt** - Password hashing and encryption
- **CORS** - Cross-origin resource sharing
- **dotenv** - Environment variable management

## 📁 Project Structure

```
expense-tracker/
├── Frontend/                 # React frontend application
│   ├── src/
│   │   ├── components/       # Reusable UI components
│   │   │   ├── common/      # Shared components
│   │   │   ├── forms/       # Form components
│   │   │   ├── layout/      # Layout components
│   │   │   └── ui/          # Pure UI components
│   │   ├── features/        # Feature-based modules
│   │   │   ├── auth/        # Authentication features
│   │   │   ├── dashboard/   # Dashboard components
│   │   │   ├── expenses/    # Expense management
│   │   │   └── income/      # Income management
│   │   ├── hooks/           # Custom React hooks
│   │   ├── services/        # API services
│   │   ├── store/           # Context API state management
│   │   ├── utils/           # Utility functions
│   │   ├── assets/          # Static assets
│   │   └── styles/          # Global styles
│   └── public/              # Public assets
├── Backend/                 # Node.js backend API
│   ├── controllers/         # Route controllers
│   ├── models/             # Database models
│   ├── routes/             # API routes
│   ├── middleware/         # Custom middleware
│   └── db/                 # Database configuration
└── README.md
```

## 🚀 Getting Started

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local or MongoDB Atlas)
- npm or yarn package manager

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/expense-tracker-plus.git
cd expense-tracker-plus
```

2. **Setup Backend**
```bash
cd Backend
npm install
```

3. **Setup Frontend**
```bash
cd ../Frontend
npm install
```

4. **Environment Variables**
Create a `.env` file in the Backend directory:
```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
```

### Running the Application

1. **Start Backend Server**
```bash
cd Backend
npm start
```

2. **Start Frontend Development Server**
```bash
cd Frontend
npm start
```

3. **Access the Application**
- Frontend: `http://localhost:3000`
- Backend API: `http://localhost:5000`

## 📱 Features in Detail

### Authentication System
- Secure user registration and login
- JWT token-based authentication
- Protected routes requiring authentication
- Automatic session management

### Financial Dashboard
- Real-time balance calculation
- Visual charts showing spending patterns
- Quick access to recent transactions
- Summary cards for key metrics

### Transaction Management
- Add income with categories and descriptions
- Add expenses with detailed categorization
- Edit and delete transactions
- Search and filter capabilities

### Reporting & Analytics
- Generate comprehensive reports
- Export data to Excel format
- Visual analytics with multiple chart types
- Historical trend analysis

## 🎨 UI/UX Features

- **Modern Design** - Clean and professional interface
- **Responsive Layout** - Works on all device sizes
- **Interactive Elements** - Hover effects and smooth transitions
- **Color-coded Categories** - Visual distinction for different expense types
- **Loading States** - User feedback during data operations
- **Error Handling** - Graceful error messages and recovery

## 🔧 API Endpoints

### Authentication
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `GET /api/auth/profile` - Get user profile

### Income Management
- `GET /api/income` - Get all income records
- `POST /api/income` - Add new income
- `DELETE /api/income/:id` - Delete income record

### Expense Management
- `GET /api/expenses` - Get all expense records
- `POST /api/expenses` - Add new expense
- `DELETE /api/expenses/:id` - Delete expense record

## 🔮 Future Enhancements

- [ ] Budget planning and tracking
- [ ] Recurring income/expense management
- [ ] Multi-currency support
- [ ] Advanced filtering and search
- [ ] Goal setting and progress tracking
- [ ] Email notifications and reminders
- [ ] Data backup and sync
- [ ] Advanced analytics and insights

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Your Name**
- GitHub: [@yourusername](https://github.com/yourusername)
- LinkedIn: [Your LinkedIn](https://linkedin.com/in/yourprofile)

## 🙏 Acknowledgments

- MongoDB for the robust database solution
- React team for the amazing frontend library
- Chart.js for beautiful data visualization
- All contributors and the open-source community

---

⭐ **Star this repository if you found it helpful!** ⭐
