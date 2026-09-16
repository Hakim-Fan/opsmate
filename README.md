# 🐬 OpsMate - Official Support & Feedback Center

<p align="center">
  <strong>A Pure, Secure, and High-Performance Mobile MySQL Client for Urgent On-Call & Data Operations</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-iOS%20%7C%20Android-green?logo=apple&logoColor=white" alt="Platform">
  <img src="https://img.shields.io/badge/Data%20Privacy-Zero%20Telemetry-blue" alt="Privacy">
  <img src="https://img.shields.io/badge/Security-AES--256%20%2B%20Biometrics-orange" alt="Security">
  <img src="https://img.shields.io/badge/Community-GitHub%20Issues-brightgreen" alt="Community">
</p>

<p align="center">
  <a href="README.zh.md">简体中文</a> •
  <a href="README.md">English</a>
</p>

---

## 📌 Repository Notice

This repository serves as the official **Support Center, Issue Tracker, and Product Documentation** for **OpsMate** (**application source code is not hosted here**).

If you encounter bugs, unexpected crashes, or have feature suggestions, please feel free to open a [GitHub Issue](https://github.com/Hakim-Fan/opsmate/issues). Our team actively reviews community feedback!

---

## 📖 About OpsMate

When production incidents strike while away from your workstation, commuting, or on vacation, DBAs and backend engineers need a dedicated tool to **pull out their phone, connect securely to their MySQL databases, and troubleshoot issues immediately**.

**OpsMate** is an offline-first mobile MySQL client designed specifically for smartphone touchscreens. Built upon two uncompromised principles—**Offline-First** and **Zero Telemetry**—it provides a dependable, high-efficiency database management and AI-assisted troubleshooting experience right in your pocket.

---

## ✨ Key Highlights

### 🔒 Uncompromising Security & Zero Telemetry
- **Direct Client-to-Server Connection**: Operates entirely client-side without any intermediary relay servers. Your device connects directly to your MySQL instance.
- **Hardware-Backed Encryption**: Sensitive credentials (database passwords, private AI API keys) are protected with a 256-bit encryption key derived from system-level hardware primitives (iOS Keychain / Android KeyStore) and stored securely in an encrypted Hive box.
- **Biometric App Lock**: Integrated native biometric authentication (Face ID, Touch ID, Android BiometricPrompt) to safeguard database configurations from unauthorized physical access.

### ⚡️ Mobile-Optimized SQL Console
- **Syntax Highlighting & Shortcut Bar**: Designed specifically for mobile screens with intelligent keyword coloring and a dedicated auxiliary keyboard bar for rapid symbol input.
- **High-Performance Data Grid (PlutoGrid)**: Smoothly view large datasets with virtualized scrolling, column resizing, and pagination.
- **SQL Snippets Manager**: Save frequently used queries and emergency diagnostic scripts for instant one-tap retrieval.
- **Connection Guard**: Built-in connection timeouts and automated idle disconnection to conserve battery life and free up database thread pools.

### 📊 Intuitive Table & Record Management
- **Instant Table Lookup**: Rapidly filter and inspect database tables, schemas, and column definitions.
- **Row-Level Visual Editor**: Easily inspect row details, insert new records, update values, and delete rows on the go.

### 🤖 Built-in AI Copilot (Bring Your Own Key)
- **BYOK Architecture**: Seamlessly configure and connect to any OpenAI-compatible API (OpenAI, DeepSeek, Claude, Ollama, etc.).
- **Direct HTTPS Communication**: AI queries and optional schema context are transmitted directly from your mobile device to your configured AI provider over HTTPS without passing through any intermediate server.
- **Smart Scenarios**: Natural language to SQL generation, instant query error explanation, slow-query index suggestions, and table schema comprehension.

### 🌐 Modern UX & Bilingual Support
- **Adaptive Appearance**: Polished design system supporting both Dark and Light modes with seamless system switching.
- **Full Internationalization**: Complete native support for both English and Simplified Chinese (简体中文).

---

## 📥 Download & Installation

- **iOS Users**: Search for **`MysqlOps`** on the App Store

---

## 💡 Feedback & Support Guidelines

We deeply value your feedback to help improve OpsMate:

### 1. Bug Reports
If you encounter unexpected behavior or app crashes, please open an [Issue](https://github.com/Hakim-Fan/opsmate/issues) with the following details:
- Device model and OS version (e.g., iPhone 15 Pro, iOS 18.2 / Pixel 8, Android 15)
- App version (check in "Settings -> App Version")
- Detailed reproduction steps and screenshots (please mask sensitive database IPs and private production data)

### 2. Feature Requests
If you would like to suggest new capabilities (e.g., SSH tunnel support, additional export formats, support for more database engines), feel free to open an issue describing your use case.

---

## ❓ Frequently Asked Questions (FAQ)

<details>
<summary><strong>Q1: Are my database credentials or query data uploaded to your servers?</strong></summary>
<p><strong>Absolutely not.</strong> OpsMate is a standalone client utility. We operate no cloud proxy servers and embed zero tracking or telemetry SDKs. Connections are established directly between your phone and your database, with passwords encrypted locally via system hardware security primitives (Keychain/KeyStore).</p>
</details>

<details>
<summary><strong>Q2: Does the AI feature expose my database schema or data?</strong></summary>
<p>The AI feature uses a Bring-Your-Own-Key (BYOK) architecture that interacts directly with your designated AI provider (e.g., OpenAI, DeepSeek) over HTTPS. No intermediary server is involved. We advise avoiding submitting unmasked, highly sensitive production records into third-party AI models.</p>
</details>

<details>
<summary><strong>Q3: Which database engines are supported?</strong></summary>
<p>Standard MySQL 5.7+, MySQL 8.0+, MariaDB, and other cloud database services compatible with MySQL wire protocol (AWS RDS, Aliyun RDS, Tencent Cloud CDB, etc.).</p>
</details>

---

<p align="center">
  Crafted by the <strong>OpsMate Team</strong> • Thank you for your support and feedback ❤️
</p>
