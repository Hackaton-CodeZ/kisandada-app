# Kisan Dada: Your AI Farming Companion

**Guiding Farmers with the Power of Intelligence.**

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)

Kisan Dada is a revolutionary mobile application designed to empower farmers with immediate access to agricultural knowledge and support. Leveraging the power of AI, this app acts as a trusted friend ("Dada" means elder brother) that farmers can turn to for advice on crop management, disease diagnosis, market prices, and more. With a multilingual interface and intuitive voice and chat options, Kisan Dada aims to bridge the information gap in the agricultural sector.

## ✨ Key Features

*   **🤖 AI-Powered Chatbot:** Get instant, location-aware answers to your farming questions. Ask about crop cycles, fertilization, pest control, and more.
*   **🗣️ Voice Interaction:** "Call" Dadaji for a hands-free, conversational experience. Perfect for getting information while in the field.
*   **🌍 Multi-Language Support:** The app is fully localized in **English**, **Hindi (किसान दादा)**, and **Kannada (ಕಿಸಾನ್ ದಾದಾ)**.
*   **📸 Image-Based Queries:** Snap a photo of your crop, and our AI will help identify potential diseases or nutrient deficiencies.
*   **🔒 Secure Authentication:** Simple and secure login using your phone number and a one-time password (OTP).
*   **💡 Smart Suggestions:** The chatbot provides helpful follow-up questions to guide your query.
*   **🔧 Farmer's Toolkit:** Access information on nearby government fertilizer shops, warehouses, and predicted market (Mandi) prices.


## 🛠️ Tech Stack

*   **Framework:** React Native (Expo)
*   **Authentication:** Firebase Authentication
*   **Real-time Communication:** WebSockets for the voice call feature. ( inprogress)
*   **API Communication:** Axios
*   **Localization:** i18next
*   **Device APIs:** Expo Location, Expo AV, Expo Image Picker, Expo File System

## 🚀 Getting Started

Follow these instructions to set up and run the project on your local machine.

### Prerequisites

*   Node.js (LTS version recommended)
*   npm or yarn
*   Expo Go app on your mobile device or an Android/iOS emulator.

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/kisan-dada.git
    cd kisan-dada
    ```

2.  **Install dependencies:**
    ```bash
    npm install
    ```

3.  **Set up Firebase:**
    *   Create a Firebase project at [firebase.google.com](https://firebase.google.com/).
    *   Enable Phone Number authentication in the "Authentication" section.
    *   From your project settings, get your Firebase configuration object.
    *   Update the configuration in `src/database/firebase.js`.

4.  **Run the application:**
    ```bash
    npx expo start
    ```
    Scan the QR code with the Expo Go app on your phone.

## 📂 Project Structure

```
.
├── assets/              # Static assets like images, fonts, and sounds
├── src/
│   ├── constants/       # Global constants (colors, dimensions)
│   ├── database/        # Firebase configuration and local DB setup
│   ├── locales/         # Language JSON files for localization
│   ├── navigation/      # React Navigation setup
│   └── screens/         # All application screens
├── App.js               # Main entry point of the application
└── README.md            # This file
```

## 🌐 Localization

Adding a new language or modifying existing text is straightforward:

1.  Go to the `src/locales/` directory.
2.  Add a new file (e.g., `ta.json` for Tamil) or edit an existing one (`en.json`, `hi.json`, `kn.json`).
3.  Add the key-value pairs for the text you want to translate.
4.  Import the new language file and add it to the resources in `src/locales/i18n.js`.
5.  Update the `languages` array in `src/screens/SelectLanguage.js`.

---

Thank you for your interest in Kisan Dada!

