# 🐬 OpsMate (OpsMate) - 官方支持与用户反馈中心

<p align="center">
  <strong>一款纯粹、安全、高效的移动端 MySQL 应急排查与数据库管理工具</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-iOS%20%7C%20Android-green?logo=apple&logoColor=white" alt="Platform">
  <img src="https://img.shields.io/badge/Data%20Privacy-Zero%20Telemetry-blue" alt="Privacy">
  <img src="https://img.shields.io/badge/Security-AES--256%20%2B%20Biometrics-orange" alt="Security">
  <img src="https://img.shields.io/badge/Community-GitHub%20Issues-brightgreen" alt="Community">
</p>

<p align="center">
  <a href="README.md">简体中文</a> •
  <a href="README.md">English</a> •
</p>

---

## 📌 仓库说明 (Repository Notice)

本仓库为 **OpsMate** 的官方用户反馈中心、问题跟进平台与文档主页（**不包含应用源代码**）。

如果您在使用过程中遇到任何问题、崩溃异常，或有好的产品建议、功能需求，欢迎随时在此提交 [Issue](https://github.com/Hakim-Fan/opsmate/issues)。团队会定期查看并跟进处理！

---

## 📖 关于 OpsMate (About)

在突发线上故障、休假外出或离开工位时，DBA 和后端开发者常常需要一种能够**随时掏出手机、迅速安全直连数据库并进行应急排查与数据定位**的专业工具。

**OpsMate** 是一款专注于移动端触控与交互体验的专业 MySQL 客户端。坚持**“离线优先（Offline-First）”**与**“零数据收集（Zero Telemetry）”**两大原则，为开发者提供随身携带的数据库排查与 AI 智能运维辅助体验。

---

## ✨ 核心功能亮点 (Highlights)

### 🔒 极致的本地数据安全与隐私保护
- **纯客户端本地直连**：不设任何自建中转服务器，手机直接与您指定的 MySQL 实例建立加密通信。
- **硬件级密码与凭据加密**：数据库密码、私有 API Key 等敏感信息，均通过系统底层设施（iOS Keychain / Android KeyStore）派生密钥，在本地沙箱内采用高强度 AES-256 加密保存。
- **生物识别应用锁**：原生支持 Face ID、Touch ID 与 Android 指纹认证，借用手机无泄露风险。

### ⚡️ 移动端专属 SQL 交互控制台
- **SQL 语法高亮与辅助键盘**：针对手机窄屏特别优化，配备快捷常用符号输入栏与代码段模板。
- **高性能表格呈现（PlutoGrid）**：轻松流畅查看海量查询结果，支持横竖屏自适应、列宽调整与分页展示。
- **常用 SQL 收藏片段（Snippets）**：一键保存常用排查语句与运维脚本，告别在手机上手打长篇 SQL。
- **连接资源守护**：内置空闲自动断开（Idle Timeout）与超时保护，避免占用数据库连接池。

### 📊 直观的数据表与记录管理
- **表级快速检索**：快速搜索与切换库内数据表，直观查看表结构 Schema。
- **数据行级可视化查看与编辑**：支持数据增、删、改、查，以及单行详细数据查看，紧急修复脏数据更轻松。

### 🤖 自带密钥的 AI 智能助手（BYOK AI Copilot）
- **自带密钥模式（Bring Your Own Key）**：支持自主配置 OpenAI、DeepSeek、Claude 等任意兼容 OpenAI 协议的大模型服务。
- **端到端直接交互**：查询内容直接由手机 HTTPS 发往您配置的模型服务商，中间无任何中继服务器。
- **智能排查场景**：自然语言生成 SQL、执行报错即时诊断、慢查询调优建议与表结构辅助解读。

### 🌐 现代体验与多语言
- **深浅色模式自适应**：精心调校的界面风格，完美适配夜间与暗黑模式。
- **多语言原生支持**：支持简体中文与英文无缝切换，支持跟随系统。

---

## 📥 获取与下载 (Download & Install)

- **iOS 用户**：App Store 搜索 **`MysqlOps`**

---

## 💡 如何提交反馈与建议 (Feedback & Support)

我们非常重视每一位开发者的使用体验，欢迎通过以下方式参与产品改进：

### 1. 提交 Bug 报告 (Bug Report)
如果您发现了功能缺陷或应用崩溃，请前往 [New Issue](https://github.com/Hakim-Fan/opsmate/issues) 并尽量附带以下信息：
- 设备机型与系统版本（如 iPhone 15 Pro, iOS 18.2 / 小米 14, Android 15）
- 应用版本号（可在应用内「设置 - 应用版本」查看）
- 问题的详细复现步骤与现象截图（请注意打码遮蔽敏感的生产数据库 IP 与业务数据）

### 2. 提出新功能需求 (Feature Request)
如果您希望增加某些操作功能（例如：支持 SSH 隧道跳板机连接、支持更多导出格式、支持更多数据库类型等），欢迎在 Issues 中开帖详细描述您的使用场景。

---

## ❓ 常见问题 (FAQ)

<details>
<summary><strong>Q1: 我的数据库密码和查询数据会被上传到你们的服务器吗？</strong></summary>
<p><strong>绝对不会。</strong> OpsMate 是一款纯客户端应用，我们没有任何中转服务器，甚至没有部署任何用户行为埋点 SDK。所有数据库连接均由您的手机直连目标服务器，密码在本地通过系统级安全设施（Keychain/KeyStore）加密保护。</p>
</details>

<details>
<summary><strong>Q2: AI 功能会泄露我的数据库数据吗？</strong></summary>
<p>本应用的 AI 功能为 BYOK（用户自带 Key）模式，直连您自己配置的 AI 服务商（如 OpenAI 或 DeepSeek），不经过任何第三方中转。您可以自主选择是否发送表结构辅助分析；为了安全起见，建议避免向 AI 模型发送未脱敏的生产环境真实业务敏感数据。</p>
</details>

<details>
<summary><strong>Q3: 支持连接哪些数据库？</strong></summary>
<p>全面支持标准 MySQL 5.7+、MySQL 8.0+ 以及 MariaDB 等兼容 MySQL 通信协议的数据库（包括自建机房、AWS RDS、阿里云 RDS、腾讯云 CDB 等）。</p>
</details>

---

<p align="center">
  由 <strong>OpsMate 团队</strong> 倾心打造 • 期待您的宝贵反馈与支持 ❤️
</p>
