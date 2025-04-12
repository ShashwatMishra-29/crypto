# 💰 Currency Monitoring App – Real-Time Crypto Tracker

A simple and elegant Flutter application for monitoring real-time cryptocurrency prices. Powered by the [CoinGecko API](https://www.coingecko.com/), this app allows users to view live rates, toggle between dark/light themes, and mark favorite cryptocurrencies for quick access.

---

## 🚀 Features

- 📊 **Live Cryptocurrency Prices**
  - Fetched from CoinGecko API
  - Includes name, price, symbol, and market cap data

- ⭐ **Favorites Management**
  - Mark cryptocurrencies as favorites
  - View your personalized list in one place

- 🌗 **Light & Dark Mode Support**
  - Seamless toggle between themes for better UI experience

- 📱 **Clean and Responsive UI**
  - Built with Flutter for Android and iOS

---

## 🛠️ Tech Stack

- **Flutter** – Cross-platform UI toolkit
- **CoinGecko API** – Free real-time cryptocurrency data
- **Provider / Riverpod / GetX** – For state management (if used)
- **Shared Preferences** – To persist favorites and theme settings (if applicable)

---

## 📦 Getting Started

### Prerequisites

- Flutter SDK installed
- An emulator or physical device connected

### Installation


git clone https://github.com/your-username/currency-monitoring-app.git
cd currency-monitoring-app
flutter pub get
flutter run
🔗 API Details
CoinGecko API Endpoint
http

GET https://api.coingecko.com/api/v3/coins/markets?vs_currency=usd
Data Returned Includes:

id, symbol, name

current_price

market_cap_rank

price_change_percentage_24h

image (for logos/icons)

📁 Folder Structure

lib/
├── main.dart
├── models/
│   ├── crypto_model.dart
│   ├── user_model.dart
│   └── favorite_model.dart
├── services/
│   ├── api_service.dart         # CoinGecko
│   ├── auth_service.dart        # Directus Auth
│   ├── favorite_service.dart    # Directus Favorites CRUD
├── providers/
│   ├── auth_provider.dart
│   ├── crypto_provider.dart
│   └── theme_provider.dart
├── screens/
│   ├── splash_screen.dart
│   ├── login_screen.dart
│   ├── signup_screen.dart
│   ├── home_screen.dart
│   ├── favorites_screen.dart
├── widgets/
│   └── crypto_card.dart
│   └── crypto_favorites_card.dart
└── theme/
    └── app_theme.dart
📸 Screenshots (Provided in another branch of same repo)
Home Screen	Dark Mode	Favorites
🤝 Contributing
Feel free to open issues or submit pull requests to improve the app. Feedback and suggestions are always welcome!

📄 License
This project is licensed under the MIT License.
