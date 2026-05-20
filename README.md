# Jay Barbers - Premium Barbershop Booking Application

A modern, user-friendly barbershop booking application with premium design. Built with Android (Kotlin + Jetpack Compose) frontend and Node.js/Express backend with MySQL database.

## ✨ Features

### User Features
- 🎨 Beautiful Material Design 3 UI with premium gold theme
- 🔐 Secure Authentication (Sign up/Login)
- 👨‍💼 Browse Barbers with ratings and reviews
- 💇 Browse Services and pricing
- 📅 Advanced Booking System with date & time slots
- 📋 Booking History & Management
- ⭐ Ratings & Reviews system
- 🔔 Push Notifications
- 💳 Payment Integration ready (Stripe)
- 👤 Profile Management

### Admin Features
- 🧑‍💼 Barber Management
- ✂️ Service Management
- 📊 Booking Management
- 📈 Analytics Dashboard
- ⭐ Customer Reviews Management

## 📱 Tech Stack

**Frontend (Android):**
- Kotlin
- Jetpack Compose
- Material Design 3
- Retrofit (HTTP Client)
- Room Database (Local Storage)
- DataStore (Preferences)
- Coil (Image Loading)

**Backend:**
- Node.js & Express.js
- MySQL Database
- JWT Authentication
- Stripe Payment Integration
- Nodemailer (Email)

## 🚀 Project Structure

```
jaybarbers/
├── android/                          # Android Application
│   ├── app/
│   │   ├── src/main/
│   │   │   ├── kotlin/com/jaybarbers/app/
│   │   │   │   ├── MainActivity.kt
│   │   │   │   ├── ui/
│   │   │   │   │   ├── screens/     # All UI Screens
│   │   │   │   │   └── theme/       # Colors & Typography
│   │   │   │   └── navigation/      # Navigation setup
│   │   │   └── AndroidManifest.xml
│   │   └── build.gradle
│   ├── settings.gradle
│   └── build.gradle
├── backend/                          # Node.js Backend
│   ├── src/
│   │   ├── routes/                  # API Routes
│   │   │   ├── auth.js              # Authentication
│   │   │   ├── barbers.js           # Barber endpoints
│   │   │   ├── services.js          # Service endpoints
│   │   │   ├── bookings.js          # Booking endpoints
│   │   │   ├── reviews.js           # Review endpoints
│   │   │   ├── payments.js          # Payment endpoints
│   │   │   └── users.js             # User profile endpoints
│   │   └── index.js                 # Main server file
│   ├── package.json
│   └── .env.example
├── database/
│   └── schema.sql                    # MySQL Database schema
├── .github/workflows/
│   └── android-build.yml             # CI/CD Pipeline
└── README.md
```

## 🎯 Setup Instructions

### Prerequisites
- Android Studio (latest version)
- Node.js v14+
- MySQL 5.7+
- Git

### 1. Android Setup

```bash
# Clone repository
git clone https://github.com/Fetizanan/jaybarbers.git
cd jaybarbers

# Open Android folder in Android Studio
open android/
```

- Build and run the app on Android Studio
- Update API endpoint in code if needed

### 2. Backend Setup

```bash
# Navigate to backend
cd backend

# Install dependencies
npm install

# Create .env file
cp .env.example .env

# Edit .env with your configuration
```

### 3. Database Setup

```bash
# Login to MySQL
mysql -u root -p

# Run schema
source database/schema.sql
```

### 4. Start Backend

```bash
cd backend
npm start
# Server runs on http://localhost:3000
```

## 📝 API Endpoints

### Authentication
- `POST /api/v1/auth/register` - User registration
- `POST /api/v1/auth/login` - User login

### Barbers
- `GET /api/v1/barbers` - Get all barbers
- `GET /api/v1/barbers/:id` - Get barber details

### Services
- `GET /api/v1/services` - Get all services
- `GET /api/v1/services/:id` - Get service details

### Bookings
- `POST /api/v1/bookings` - Create booking
- `GET /api/v1/bookings/user/:user_id` - Get user bookings
- `GET /api/v1/bookings/slots/:barber_id/:date` - Get available slots

### Reviews
- `POST /api/v1/reviews` - Create review
- `GET /api/v1/reviews/barber/:barber_id` - Get barber reviews

### Payments
- `POST /api/v1/payments` - Process payment

## 🎨 Design Highlights

- **Premium Color Scheme**: Dark navy with gold accents
- **Modern UI**: Material Design 3 with smooth animations
- **Responsive Layout**: Adapts to all screen sizes
- **User-Friendly**: Intuitive navigation and clear CTAs
- **Accessible**: Proper contrast ratios and readable text

## 📱 Screens Included

1. **Splash Screen** - App intro
2. **Login Screen** - User authentication
3. **Register Screen** - New user signup
4. **Home Screen** - Main dashboard with featured barbers & services
5. **Barbers Screen** - Browse all barbers
6. **Barber Detail Screen** - View barber info & services
7. **Booking Screen** - Select date, time & confirm appointment
8. **Bookings Screen** - View booking history
9. **Profile Screen** - User profile management

## 🔐 Security Features

- JWT Token Authentication
- Password Hashing (bcryptjs)
- Input Validation
- CORS Protection
- Secure API endpoints

## 📦 Dependencies

See `backend/package.json` and `android/app/build.gradle` for complete dependency lists.

## 🚀 Deploy

### Android
- Build APK: `./gradlew assembleRelease`
- Build Bundle: `./gradlew bundleRelease`
- Deploy to Google Play Store

### Backend
- Deploy to Heroku, AWS, DigitalOcean, or any Node.js hosting
- Setup environment variables
- Configure MySQL database

## 📄 License

MIT License - feel free to use this project!

## 👨‍💻 Author

**Fetizanan** - [GitHub](https://github.com/Fetizanan)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📞 Support

For issues or questions, please open a GitHub issue.

---

**Made with ❤️ for a premium barbershop experience**
