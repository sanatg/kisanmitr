# 🌾 Kisan Mitra (किसान मित्र)

A hyper-personalized mobile AI companion for the modern Indian farmer, developed by **Code Crew** for the **Smart India Hackathon 2025**.

---

## 🎯 The Problem
Small and marginal farmers in India face a critical information gap that leads to:
- Reduced yields  
- Lower profitability  
- Increased risks from climate volatility and sub-optimal practices  

Access to timely advice, transparent market data, and effective pest management is often fragmented and inaccessible.

---

## ✨ Our Solution
**Kisan Mitra** is a one-stop mobile application that bridges this gap.  
It acts as a true friend to the farmer by providing a **hyper-personalized, AI-driven platform** that consolidates:
- Crop advice  
- Pest management  
- Weather forecasts  
- Government schemes  

into a single, intuitive interface.  

💡 **Mission**: Transform raw data into actionable wisdom, empowering farmers to increase yield, optimize resources, and improve livelihoods.

---

## 🚀 Key Features
- 🤖 **Personalized AI Assistant**:  
  Custom-trained agricultural LLM analyzes soil type, pH, satellite imagery, and weather for predictive crop recommendations.

- 📸 **Image-Based Disease Diagnosis**:  
  Farmers can upload a photo of an affected plant for instant diagnosis and low-cost remedies.

- 🗣️ **Multilingual Conversational Interface**:  
  Voice-based Q&A in native languages (Hindi, Bengali, English, etc.) to overcome literacy barriers.

- 🌦️ **Hyper-Local Weather**:  
  Real-time, farm-specific weather data and advisories.

- 🌐 **Offline-First Capability**:  
  Critical features like pest diagnosis and FAQs work without internet.

- 📄 **Government Schemes**:  
  Simplified, centralized access to the latest schemes and subsidies.

- 📊 **Personalized Dashboard**:  
  A clean interface showing farm status, weather, and upcoming tasks.

---

## 🛠️ Technical Architecture

### Frontend: The User Experience
- **Framework**: React Native  
- **Why?** Cross-platform (Android & iOS), rapid development, and native-like performance.

### Intelligence & Data Layer: The Brains
- **AI Core**: Custom-Trained Agricultural LLM (backend)  
- **Data Sources**:  
  - **Bhuvan API** → Soil parameters (pH, moisture)  
  - **OpenWeather API** → Live meteorological data  

---

## 💡 Innovation: Offline-First Capability
- **On-Device AI**: MiniCPM (lightweight LLM)  
- **Why?** Rural connectivity is unreliable.  
- **Fallback Functions**: Image-based pest diagnosis + basic queries directly on the phone.  

---

## ⚙️ System Flow
- **With Internet**:  
  - React Native app → Hono backend → Custom LLM  
  - Data caching: Redis  
  - Persistent storage: Firebase  
  - External APIs: Bhuvan + OpenWeather  

- **Without Internet**:  
  - App uses on-device **MiniCPM LLM**  
  - Offline Firebase DB provides essential functionality  

---

## 🏁 Getting Started


# Clone the repository
git clone https://github.com/your-repo/kisan-mitra.git
cd kisan-mitra

# Install dependencies
npm install

# Run the application on Android
npx react-native run-android

# Run the application on iOS
npx react-native run-ios
