# 🍎 Release Predictor of OS by Apple

**Predict the future of Apple operating systems — with just a version number.**

> This project uses polynomial regression models to predict the release dates of Apple OSs (iOS, macOS, watchOS, visionOS, etc.) based on past data.

---

## 🔍 Features | 特性一览

- 🧠 **AI-Based Date Prediction** — Input an iOS version (like `16.1`), and the model estimates its release date.
- 🌐 **Cross-Platform Mapping** — Instantly see equivalent versions for:
  - iPadOS
  - tvOS
  - macOS
  - watchOS
  - visionOS
- 🪞 **未来版本预测** — 显示距离最近的未来主版本信息。
- 📎 **Useful Apple Dev Resources** — 一键跳转到 Apple 官方设计与开发文档。

---

## 🚀 Live Demo | 在线体验

👉 [Try it here](https://borancui.site/PredictAppleOSVersion)  
👨‍💻 Developed by [Boran Cui](https://borancui.site)

---

## 🧠 How it works | 工作原理简述

The site loads a set of trained models from `models.json`, each fitting a version range with its own linear regression:

```js
predictedDays = coef * versionNumber + intercept
releaseDate = minDate + predictedDays
```

---

## 📁 Project Structure | 项目结构

```
📦 PredictAppleOSVersion
├── index.html            # Main UI and logic
├── models.json           # Release prediction models
├── images/               # Assets and icons
└── styles/               # Embedded in HTML (for now)
```

**“Apple doesn’t tell you the date. But now, you know.” 🍏**
