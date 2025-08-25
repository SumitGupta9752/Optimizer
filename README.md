# Smart Kisan 🌾
## IoT & AI-Enabled Agricultural Assistant

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Android](https://img.shields.io/badge/platform-Android-green.svg)](https://developer.android.com)
[![Python](https://img.shields.io/badge/backend-Python-yellow.svg)](https://www.python.org)
[![MongoDB](https://img.shields.io/badge/database-MongoDB-green.svg)](https://www.mongodb.com)
[![Firebase](https://img.shields.io/badge/auth-Firebase-orange.svg)](https://firebase.google.com)

Smart Kisan is a comprehensive Android application that empowers farmers with intelligent agricultural solutions. By leveraging IoT sensors, AI-powered crop disease detection, and integrated e-commerce capabilities, this platform transforms traditional farming practices into data-driven agricultural management.

## 🌟 Key Features

### 📊 Real-Time Agricultural Intelligence
- **Smart Recommendations**: Personalized farming advice based on real-time environmental data
- **IoT Integration**: Continuous monitoring through soil moisture, temperature, and humidity sensors
- **Weather Analytics**: Localized weather forecasts with agricultural impact analysis
- **Crop Health Monitoring**: Track plant growth patterns and environmental conditions

### 🤖 AI-Powered Disease Detection
- **Image Recognition**: Advanced computer vision for instant crop disease identification
- **Pest Detection**: Early warning system for common agricultural pests
- **Treatment Recommendations**: Specific solutions based on detected issues
- **Predictive Analytics**: Proactive alerts before problems escalate

### 🛒 Integrated E-Commerce Platform
- **Treatment Products**: Direct access to verified agricultural supplies
- **Local Vendor Network**: Connect with nearby agricultural retailers
- **Price Comparison**: Compare costs across multiple suppliers
- **Order Tracking**: Monitor delivery status of purchased products

### 👤 User Management System
- **Secure Authentication**: Firebase-powered login and registration
- **Farm Profiles**: Manage multiple farm locations and crop varieties
- **Historical Data**: Comprehensive farming activity logs and analytics
- **Personalized Dashboard**: Customized interface based on farm requirements

## 🛠️ Technology Stack

### Frontend Development
```
Platform: Android (Native)
Language: Java
IDE: Android Studio
UI Framework: Material Design Components
Authentication: Firebase Auth SDK
```

### Backend Architecture
```
Language: Python
Web Framework: Flask/FastAPI
Database: MongoDB
Cloud Services: Firebase Cloud Functions
API Design: RESTful APIs
```

### AI/ML Implementation
```
Framework: TensorFlow/Keras
Model: Convolutional Neural Networks (CNN)
Image Processing: OpenCV
Model Deployment: TensorFlow Lite for mobile
```

### IoT Integration
```
Sensors: DHT22 (Temperature/Humidity), Soil Moisture Sensors
Connectivity: WiFi/Bluetooth protocols
Data Processing: Real-time analytics and visualization
```

## 📋 System Architecture

```
┌─────────────────┐    ┌──────────────────┐    ┌─────────────────┐
│   Android App   │◄──►│   Backend API    │◄──►│    MongoDB      │
│   (Java/XML)    │    │   (Python)       │    │   Database      │
└─────────────────┘    └──────────────────┘    └─────────────────┘
         ▲                        ▲                       ▲
         │                        │                       │
         ▼                        ▼                       ▼
┌─────────────────┐    ┌──────────────────┐    ┌─────────────────┐
│   Firebase      │    │   AI/ML Model    │    │   IoT Sensors   │
│  Authentication │    │  Disease Detection│   │  (Environmental) │
└─────────────────┘    └──────────────────┘    └─────────────────┘
```

## 🚀 Installation & Setup

### Prerequisites
- Android Studio (Latest Version)
- Python 3.8+
- MongoDB Community Server
- Firebase Project Setup
- Git

### Backend Setup
```bash
# Clone the repository
git clone https://github.com/yourusername/smart-kisan.git
cd smart-kisan

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Configure MongoDB connection
# Update config.py with your MongoDB URI

# Set up Firebase credentials
# Add your firebase-service-account.json to the config folder

# Run the backend server
python app.py
```

### Android App Setup
```bash
# Open Android Studio
# Import the android-app folder as a new project

# Configure Firebase
# Add google-services.json to app/ directory

# Update API endpoints
# Modify API_BASE_URL in Constants.java

# Build and run the application
```

### AI Model Setup
```bash
# Navigate to ML directory
cd ml-models

# Download pre-trained weights (if available)
# Or train the model using provided datasets

# Convert model for mobile deployment
python convert_to_tflite.py

# Copy model files to Android assets folder
```

## 📱 App Screenshots

| Feature | Screenshot | Description |
|---------|------------|-------------|
| **Dashboard** | ![Dashboard](screenshots/dashboard.png) | Real-time farm overview with sensor data |
| **Disease Detection** | ![Disease](screenshots/disease-detection.png) | AI-powered crop disease identification |
| **E-commerce** | ![Shop](screenshots/ecommerce.png) | Integrated marketplace for farm supplies |
| **IoT Monitoring** | ![IoT](screenshots/iot-dashboard.png) | Live sensor data visualization |

## 🔧 API Documentation

### Authentication Endpoints
```
POST /api/auth/login      - User authentication
POST /api/auth/register   - New user registration
GET  /api/auth/profile    - User profile information
```

### Agricultural Data Endpoints
```
GET  /api/crops           - Fetch crop information
POST /api/crops/analyze   - Submit crop image for analysis
GET  /api/weather         - Weather data and forecasts
GET  /api/sensors         - IoT sensor data
```

### E-commerce Endpoints
```
GET  /api/products        - Available agricultural products
POST /api/orders          - Place new order
GET  /api/orders/:id      - Order tracking
```

## 🧪 Testing

### Backend Testing
```bash
# Run unit tests
python -m pytest tests/

# Run integration tests
python -m pytest tests/integration/

# API testing with coverage
pytest --cov=app tests/
```

### Android Testing
```bash
# Run unit tests in Android Studio
./gradlew test

# Run instrumentation tests
./gradlew connectedAndroidTest
```

## 🚀 Deployment

### Backend Deployment
- **Cloud Platform**: AWS/Google Cloud/Heroku
- **Database**: MongoDB Atlas (Cloud)
- **CI/CD**: GitHub Actions for automated deployment
- **Monitoring**: Application performance monitoring setup

### Mobile App Distribution
- **Testing**: Firebase App Distribution for beta testing
- **Production**: Google Play Store deployment
- **Analytics**: Firebase Analytics integration

## 📊 Performance Metrics

- **Disease Detection Accuracy**: 92% on test dataset
- **Response Time**: < 2 seconds for API calls
- **Model Size**: < 10MB (optimized for mobile)
- **Offline Capability**: Core features available without internet

## 🤝 Contributing

We welcome contributions to Smart Kisan! Please follow these guidelines:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Development Guidelines
- Follow PEP 8 for Python code
- Use Android coding standards for Java
- Write unit tests for new features
- Update documentation for API changes

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Your Name**
- GitHub: [@yourusername](https://github.com/yourusername)
- LinkedIn: [Your LinkedIn](https://linkedin.com/in/yourprofile)
- Email: your.email@example.com

## 🙏 Acknowledgments

- Thanks to the agricultural community for feedback and testing
- Open-source libraries and frameworks used in development
- IoT hardware partners for sensor integration
- Beta testers and early adopters

## 📞 Support

For support and queries:
- 📧 Email: support@smartkisan.com
- 📱 Phone: +91-XXXXXXXXXX
- 💬 Discord: [Smart Kisan Community](https://discord.gg/smartkisan)

## 🔮 Future Roadmap

- [ ] Machine Learning model improvements
- [ ] Multi-language support
- [ ] Drone integration for aerial crop monitoring
- [ ] Blockchain-based supply chain tracking
- [ ] Voice-based interactions
- [ ] Advanced analytics dashboard
- [ ] Integration with government agricultural schemes

---

**Made with ❤️ for farmers and sustainable agriculture**
