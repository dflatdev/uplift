# 🎈 Uplift

> *Gently expand your possibilities, one day at a time*

A pacing app using **energy envelope theory** to help people with chronic fatigue, ME/CFS, Long COVID, and other energy-limiting conditions track their activity, monitor energy levels, and prevent crashes with colorful balloon-themed visualizations.

## 🌟 The Balloon Philosophy

Think of your energy like inflating a balloon:

- **Expand slowly** - Gradual, consistent effort builds capacity over time
- **Don't overinflate** - Push too hard and risk a "pop" (crash)
- **Find your balance** - Stay within your energy envelope for sustainable recovery

## ✨ Features

### 📊 Health Data Integration
- **Google Fit** (Android) and **Apple Health** (iOS) integration
- Automatic activity tracking (steps, distance, active minutes)
- Heart rate monitoring throughout the day
- Sleep data import

### 🌅 Morning Check-In
- "How did you sleep?" (quality rating)
- "How ready do you feel for today?" (energy forecast)
- Set your daily activity intention

### 🌙 Evening Reflection
- "Did you experience any crashes today?"
- Log high stressors:
  - 🤒 Illness/physical symptoms
  - 💼 Work stress
  - 👥 Social exertion
  - 😰 Emotional stress
  - 🏃 Physical overexertion

                        - ### 📅 Wee### 📅 Weekly Calendar View
- Beautiful balloon-themed visualization
- Color-coded days based on energy levels
- Activity and heart rate overlays
- Crash indicators with correlated stressors
- Pattern recognition to identify triggers

### 🎨 Balloon-Themed Design
- Colorful, uplifting UI that grows with you
- Balloons that "inflate" to show energy capacity
- Gentle animations and encouraging feedback
- Customizable color themes

## 🛠️ Tech Stack

- **Framework**: React Native with Expo
- **State Management**: Zustand
- **Health Data**:
  - `react-native-health` (Apple HealthKit)
  - `react-native-google-fit` (Google Fit API)
- **Local Storage**: AsyncStorage + SQLite
- **UI Components**: Custom themed components
- **Charts**: react-native-chart-kit / Victory Native

## 📁 Project Structure

```
uplift/
├── src/
│   ├── components/
│   │   ├── calendar/
│   │   │   ├── WeeklyCalendar.tsx
│   │   │   ├── DayCell.tsx
│   │   │   └── CrashIndicator.tsx
│   │   ├── checkin/
│   │   │   ├── MorningCheckin.tsx
│   │   │   └── EveningReflection.tsx
│   │   ├── balloon/
│   │   │   ├── BalloonGauge.tsx
│   │   │   └── BalloonAnimation.tsx
│   │   └── common/
│   ├── screens/
│   │   ├── HomeScreen.tsx
│   │   ├── CalendarScreen.tsx
│   │   ├── CheckinScreen.tsx
│   │   └── SettingsScreen.tsx
│   ├── services/
│   │   ├── healthkit/
│   │   ├── googlefit/
│   │   └── notifications/
│   ├── store/
│   │   ├── checkinStore.ts
│   │   ├── healthStore.ts
│   │   └── settingsStore.ts
│   ├── models/
│   │   ├── DailyLog.ts
│   │   ├── HealthData.ts
│   │   └── Stressor.ts
│   ├── utils/
│   │   ├── correlation.ts
│   │   └── dateHelpers.ts
│   └── theme/
│       ├── colors.ts
│       └── balloonTheme.ts
├── App.tsx
├── app.json
└── package.json
```

## 🚀 Getting Started

### Prerequisites
- Node.js 18+
- Expo CLI
- iOS Simulator / Android Emulator or physical device

### Installation

```bash
# Clone the repository
git clone https://github.com/dflatdev/uplift.git
cd uplift

# Install dependencies
npm install

# Start the development server
npx expo start
```

### Health Permissions

The app requires the following health permissions:
- **iOS**: HealthKit access for steps, heart rate, sleep
- **Android**: Google Fit access for activity and heart rate data

## 📖 Energy Envelope Theory

Energy Envelope Theory suggests that people with chronic fatigue conditions should:

1. **Identify your envelope** - Understand your available energy
2. **Stay within limits** - Avoid pushing beyond your capacity
3. **Gradual expansion** - Slowly increase activity as tolerance builds
4. **Track patterns** - Recognize what triggers crashes

Uplift helps you visualize and manage this process with intuitive balloon metaphors and data-driven insights.

## 🎯 Roadmap

- [ ] Core app structure and navigation
- [ ] Morning and evening check-in flows
- [ ] Apple HealthKit integration
- [ ] Google Fit integration
- [ ] Weekly calendar view with crash correlation
- [ ] Balloon animations and theming
- [ ] Push notification reminders
- [ ] Data export for healthcare providers
- [ ] Trend analysis and insights
- [ ] Widget support

## 🤝 Contributing

Contributions are welcome! This app is being built to help people manage chronic conditions, so thoughtful, accessible design is a priority.

## 📄 License

MIT License - see [LICENSE](LICENSE) for details.

## 💜 Acknowledgments

Built with care for the chronic illness communty. Your energy matters.

---

*Remember: Recovery isn't liner, but every gentle step counts. 🎈*
