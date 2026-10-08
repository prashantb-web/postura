# <img src="assets/logo.png" align="right" width="120" alt="Postura Logo" /> Postura

[![SemiXthon '26 Winner](https://img.shields.io/badge/SemiXthon%20'26-Winner%20🏆-FFD700?style=for-the-badge&logo=trophy&logoColor=black)](https://github.com/prashantb-web/postura)
[![Flutter](https://img.shields.io/badge/Flutter-3.10+-02569B?style=for-the-badge&logo=flutter&logoColor=white)](https://flutter.dev)
[![License: MIT](https://img.shields.io/badge/License-MIT-teal.svg?style=for-the-badge)](LICENSE)

**Postura** is an award-winning, smart posture monitoring application built with Flutter. It pairs seamlessly with an embedded hardware posture-tracking sensor over Bluetooth Low Energy (BLE) to deliver real-time spinal alignment monitoring, dynamic calibration, slouch detection alerts, and habit coaching wrapped in a modern glassmorphic interface.

---

## 🏆 Achievements & Recognition

### 🥇 Winner — SemiXthon '26 (Delhi Technological University)
**Postura** was built and showcased as a winning hardware-software solution at **SemiXthon '26**, North India's flagship hardware hackathon organized by **Semicon DTU** in collaboration with the **Vinod Dham Center of Excellence for Semiconductor and Microelectronics** at **Delhi Technological University (DTU)**.

#### 🌟 SemiXthon '26 Highlights & Impact:
- **Track Excellence**: Built under the **Healthcare & Assistive Human-Device Interface** track, combining low-power embedded hardware with a cross-platform mobile companion.
- **Hardware-Software Synergy**: Live prototype demonstration featuring real-time IMU sensor telemetry over BLE, sub-second latency posture angle streaming, dynamic user baseline calibration, and haptic feedback triggers.
- **Real-World Wellness Solution**: Addressed the epidemic of postural strain and musculoskeletal disorders among desk workers, students, and professionals through continuous, non-intrusive monitoring.

---

## ✨ Key Features

- 🖥️ **Real-Time Telemetry Dashboard**: Monitor real-time spinal inclination angles, tilt deviation, and dynamic posture health scores.
- ⚡ **Smart Calibration**: 3-second rapid calibration workflow to establish personalized "good posture" baselines tailored to each user's anatomy.
- 📡 **BLE Connectivity**: Robust Bluetooth Low Energy communication powered by `flutter_blue_plus` for ultra-low power consumption and high-frequency sensor streaming.
- 🎨 **Modern Glassmorphic UI**: Sleek dark and light themes featuring frosted glass aesthetics, vibrant teal accents, fluid micro-animations, and responsive layouts.
- 📳 **Intelligent Slouch Alerts**: Real-time multi-modal feedback (haptic vibration and visual alerts) when slouching exceeds customizable thresholds.
- 📊 **History & Habit Analytics**: Comprehensive session logs, posture trend charts, slouch frequency analytics, and daily wellness metrics.
- ⚙️ **Customizable Settings**: Fine-grained configuration for slouch angle thresholds, alert sensitivity, session goals, and device connection preferences.

---

## 🛠️ Architecture & Tech Stack

- **Framework**: [Flutter](https://flutter.dev) (Dart 3+)
- **State Management**: [Riverpod](https://riverpod.dev) (reactive, testable architecture with fine-grained dependency injection)
- **Routing**: [GoRouter](https://pub.dev/packages/go_router) (declarative shell navigation with deep linking support)
- **Local Storage**: [Hive](https://pub.dev/packages/hive) & [SharedPreferences](https://pub.dev/packages/shared_preferences) (fast offline caching of posture metrics and settings)
- **Hardware Communication**: [Flutter Blue Plus](https://pub.dev/packages/flutter_blue_plus) (cross-platform Bluetooth Low Energy BLE integration)

---

## 📂 Project Structure

```text
lib/
├── app/                  # Application routing, themes, and global initialization
├── modules/              # Feature modules
│   ├── posture/          # BLE services, calibration flow, & state notifier
│   └── storage/          # Hive local models, storage services, & preferences
├── shared/               # Reusable design system, components, & utilities
│   ├── components/       # Glassmorphic templates, charts, & custom widgets
│   └── constants/        # Design tokens, color palettes, and localized strings
└── views/                # Presentation views (Home, History, Insights, Settings)
```

---

## 🚀 Getting Started

### Prerequisites

- [Flutter SDK](https://docs.flutter.dev/get-started/install) (v3.10.7 or later)
- [Dart SDK](https://dart.dev/get-dart) (included with Flutter)
- Android or iOS device with Bluetooth Low Energy (BLE) support

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/prashantb-web/postura.git
   cd postura
   ```

2. **Install dependencies**:
   ```bash
   flutter pub get
   ```

3. **Run code generation** (for Hive models):
   ```bash
   flutter pub run build_runner build --delete-conflicting-outputs
   ```

4. **Run the application**:
   ```bash
   flutter run
   ```

---

## 🔒 License

Distributed under the MIT License. See `LICENSE` for more information.

---

<p align="center">
  Crafted with ❤️ by <a href="https://github.com/prashantb-web">Prashant Bhandari</a>
</p>
