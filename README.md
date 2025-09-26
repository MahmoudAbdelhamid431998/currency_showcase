# <img src="assets/app_icon.png" alt="Currency Converter" width="70"/> Currency Converter

<div align="center">

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![iOS](https://img.shields.io/badge/iOS-000000?style=for-the-badge&logo=ios&logoColor=white)
![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Web](https://img.shields.io/badge/Web-4285F4?style=for-the-badge&logo=google-chrome&logoColor=white)

**A comprehensive and reliable currency converter application built with Flutter**

*Providing instant, accurate exchange rates for 150+ currencies worldwide*

[Features](#-features) • [Installation](#-installation) • [Usage](#-usage) • [Architecture](#-architecture) • [Contributing](#-contributing)

</div>

---

## 📋 Description

**Currency Converter** is an essential mobile application designed to simplify global financial transactions for travelers, investors, and international business professionals. Built with Flutter, it provides real-time and accurate exchange rates with an intuitive, user-friendly interface that works seamlessly across all platforms.

### 🌟 Why Choose Currency Converter?

- **Real-time Accuracy**: Live exchange rates for 150+ currencies
- **Offline Functionality**: Works without internet connection using cached data
- **Multi-language Support**: Available in Arabic and English
- **Privacy-Focused**: No personal data collection
- **Cross-Platform**: Native experience on Android, iOS, Web, Windows, macOS, and Linux

---

## ✨ Features

### 🔄 **Core Functionality**
- **Real-time Exchange Rates**: Instant access to current exchange rates for over 150 global currencies
- **Offline Mode**: Cached exchange rates ensure functionality without internet connectivity
- **Quick Conversion**: Enter amounts and get results within seconds
- **Multi-currency Calculator**: Convert between multiple currencies simultaneously

### 🎨 **User Experience**
- **Intuitive Interface**: Clean, modern design with easy navigation
- **Country Flags**: Visual currency identification with country flags
- **Responsive Design**: Optimized for phones, tablets, and desktop
- **Dark/Light Themes**: Customizable themes including system-based switching

### ⭐ **Personalization**
- **Favorite Currencies**: Create a personalized list of frequently used currencies
- **Base Currency**: Set your preferred base currency for calculations
- **Language Support**: Full Arabic and English localization
- **Auto-refresh**: Configurable automatic rate updates

### 🛡️ **Privacy & Security**
- **No Personal Data**: Zero collection of personally identifiable information
- **Local Storage**: All preferences stored securely on your device
- **Privacy Compliant**: Fully compliant with Google Play and international privacy standards

### 🌐 **Technical Features**
- **Cross-Platform**: Native performance on all major platforms
- **Real-time Updates**: Live connectivity monitoring and automatic updates
- **Error Handling**: Robust error management with fallback mechanisms
- **Logging System**: Comprehensive logging for debugging and optimization

---

## 🛠️ Technology Stack

| Technology | Purpose | Version |
|------------|---------|----------|
| **Flutter** | Cross-platform framework | ^3.5.3 |
| **Dart** | Programming language | ^3.5.3 |
| **GetX** | State management & navigation | ^4.6.6 |
| **HTTP** | API communication | ^0.13.5 |
| **SharedPreferences** | Local data persistence | ^2.2.2 |
| **Intl** | Internationalization | ^0.19.0 |
| **Country Flags** | Flag display | ^2.2.0 |
| **Connectivity Plus** | Network status monitoring | ^5.0.2 |
| **Logger** | Logging system | ^2.0.2+1 |

### 🏗️ **Architecture**
- **Pattern**: MVC (Model-View-Controller) with GetX
- **State Management**: GetX Reactive State Management
- **API Integration**: RESTful API with error handling
- **Storage**: Local persistence with SharedPreferences
- **Internationalization**: Multi-language support with dynamic switching

---

## 📱 Screenshots

> **Note**: Screenshots will be added soon. The app features a modern, clean interface with:
> - Currency conversion screen with real-time rates
> - Settings page with theme and language options
> - Favorite currencies management
> - Responsive design for all screen sizes

---

## 🚀 Installation

### Prerequisites
- Flutter SDK (version 3.5.3 or higher)
- Dart SDK (version 3.5.3 or higher)
- Android Studio / VS Code with Flutter extensions
- Git

### 📥 **Clone the Repository**
```bash
git clone https://github.com/[your-username]/currency-converter.git
cd currency-converter
```

### 📦 **Install Dependencies**
```bash
flutter pub get
```

### 🔧 **Configure Development Environment**
1. Ensure Flutter is properly installed:
   ```bash
   flutter doctor
   ```

2. Connect your device or start an emulator

3. Verify device connectivity:
   ```bash
   flutter devices
   ```

### ▶️ **Run the Application**
```bash
# Debug mode
flutter run

# Release mode
flutter run --release

# Specific platform
flutter run -d chrome          # Web
flutter run -d windows         # Windows
flutter run -d macos           # macOS
```

### 📦 **Build for Production**
```bash
# Android APK
flutter build apk --release

# Android App Bundle
flutter build appbundle --release

# iOS
flutter build ios --release

# Web
flutter build web --release

# Windows
flutter build windows --release
```

---

## 💡 Usage

### **Basic Currency Conversion**
1. Launch the app
2. Select your base currency from the dropdown
3. Enter the amount you want to convert
4. View real-time conversion rates for all displayed currencies
5. Add or remove currencies using the + button or swipe gestures

### **Managing Favorites**
1. Navigate to the currency selection screen
2. Tap the star icon next to any currency to add it to favorites
3. Access your favorite currencies quickly from the main screen

### **Customizing Settings**
1. Tap the settings icon in the app bar
2. Choose your preferred language (Arabic/English)
3. Select theme preference (Light/Dark/System)
4. Configure auto-refresh intervals
5. Set your default base currency

### **Offline Usage**
- The app automatically caches exchange rates
- Continue using the app without internet connection
- Cached rates display with timestamps
- Automatic updates when connection is restored

---

## 🏗️ Project Architecture

```
lib/
├── controllers/           # Business logic and state management
│   ├── currency_controller.dart    # Currency conversion logic
│   └── settings_controller.dart    # App settings management
├── models/               # Data models
│   └── currency.dart     # Currency data structure
├── screens/              # UI screens
│   ├── home_screen.dart  # Main conversion interface
│   └── settings_screen.dart # Settings and preferences
├── services/             # External services
│   └── api_service.dart  # Exchange rate API integration
├── translations/         # Internationalization
│   ├── app_translations.dart # Translation mappings
│   └── translations.dart # Translation strings
├── utils/                # Utility functions
│   ├── app_logger.dart   # Logging system
│   ├── logger.dart       # Logger configuration
│   └── themes.dart       # Theme definitions
├── widgets/              # Reusable UI components
│   └── eu_flag.dart      # Custom flag widget
└── main.dart             # Application entry point
```

### **Key Components**

- **Controllers**: Handle business logic using GetX pattern
- **Services**: Manage external API calls and data fetching
- **Models**: Define data structures for type safety
- **Screens**: Implement UI layouts and user interactions
- **Utils**: Provide helper functions and configurations
- **Widgets**: Contain reusable UI components

---

## 🌐 API Integration

### **Exchange Rate Provider**
- **Service**: [ExchangeRate-API](https://exchangerate-api.com/)
- **Endpoint**: `https://open.er-api.com/v6/latest/{base_currency}`
- **Features**: 
  - Free tier with sufficient quota
  - Real-time exchange rates
  - 150+ currency support
  - Reliable uptime

### **Rate Update Strategy**
- **Auto-refresh**: Configurable intervals (default: 5 minutes)
- **Manual refresh**: Pull-to-refresh and refresh button
- **Offline fallback**: Cached rates with timestamps
- **Error handling**: Graceful degradation when API is unavailable

---

## 🌍 Internationalization

### **Supported Languages**
- **English**: Full localization
- **Arabic**: Complete RTL support with cultural adaptations

### **Adding New Languages**
1. Add translation strings to `lib/translations/translations.dart`
2. Update `lib/translations/app_translations.dart`
3. Test RTL layouts if applicable
4. Update currency names in local language

---

## 📊 Features in Detail

### **Smart Caching System**
- Automatic rate caching for offline access
- Intelligent cache invalidation
- Timestamp tracking for data freshness
- Minimal storage footprint

### **Responsive Design**
- **Mobile**: Optimized for phones with touch interactions
- **Tablet**: Sidebar layout with enhanced productivity
- **Desktop**: Full-featured experience with keyboard shortcuts
- **Web**: Progressive Web App capabilities

### **Performance Optimization**
- Lazy loading of currency data
- Efficient state management
- Minimal memory footprint
- Fast startup times

---

## 🤝 Contributing

We welcome contributions! Please follow these steps:

### **Getting Started**
1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Make your changes
4. Test thoroughly
5. Commit your changes: `git commit -m 'Add amazing feature'`
6. Push to the branch: `git push origin feature/amazing-feature`
7. Open a Pull Request

### **Development Guidelines**
- Follow Dart/Flutter best practices
- Maintain code formatting with `dart format`
- Add tests for new features
- Update documentation
- Ensure all platforms build successfully

### **Code Style**
- Use meaningful variable and function names
- Add comments for complex logic
- Follow the established project structure
- Maintain consistency with existing code

---

## 🧪 Testing

```bash
# Run all tests
flutter test

# Run with coverage
flutter test --coverage

# Integration tests
flutter drive --target=test_driver/app.dart
```

### **Test Structure**
- Unit tests for business logic
- Widget tests for UI components
- Integration tests for user workflows
- API mock tests for service layer

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Developer

**Mahmoud Abdelhamid**
- 📧 Email: [Add your email]
- 🐙 GitHub: [Add your GitHub profile]
- 💼 LinkedIn: [Add your LinkedIn profile]

---

## 🙏 Acknowledgments

- [ExchangeRate-API](https://exchangerate-api.com/) for providing reliable exchange rate data
- [Flutter Team](https://flutter.dev/) for the amazing framework
- [GetX](https://pub.dev/packages/get) for efficient state management
- [Country Flags](https://pub.dev/packages/country_flags) for beautiful flag displays
- Open source community for continuous inspiration

---

## 📈 Roadmap

### **Upcoming Features**
- [ ] Historical exchange rate charts
- [ ] Currency trend analysis
- [ ] Rate change notifications
- [ ] Export conversion history
- [ ] Widget support for quick conversions
- [ ] More language localizations

### **Technical Improvements**
- [ ] Enhanced caching strategies
- [ ] Improved error handling
- [ ] Performance optimizations
- [ ] Accessibility enhancements
- [ ] Advanced testing coverage

---

## 🐛 Issues and Support

Found a bug or have a feature request?

1. Check existing [issues](../../issues)
2. Create a new issue with detailed description
3. Include steps to reproduce (for bugs)
4. Add screenshots if applicable

---

<div align="center">

**⭐ Star this repository if you found it helpful!**

**Made with ❤️ using Flutter**

</div>
