# FitRang Chrome Extension

This Chrome Extension is a companion tool for the FitRang platform. It fetches and displays profiles the user has access to and integrates directly with the analysis service to enable seamless product analysis workflows.

---

## 🧠 Features

- 🧾 Fetches all profiles a user has access to via the `/profiles` endpoint.
- 🧪 Sends selected profile and product data to the Analysis Service.
- 🧠 Utilizes ChatGPT API for product analysis.
- 🔐 Secure communication via session-based authorization.

---

## 🚀 Getting Started

### 1. Clone the Repository

### 2. Load the Extension in Chrome

1. Open Chrome and navigate to `chrome://extensions/`
2. Enable **Developer Mode**
3. Click **"Load unpacked"**
4. Select the extension directory

---

## 🔧 Development

### Tech Stack

* JavaScript / HTML / CSS
* Chrome Extension APIs
* Axios for API requests

### Folder Structure

```
fitrang-extension/
│
├── manifest.json          # Chrome extension metadata
├── background.js          # Background script (if any)
├── popup.html             # Main UI
├── popup.js               # JS logic
├── styles.css             # Basic styles
└── utils.js               # Helper functions
```

---

## 🔐 Permissions

The extension requests the following permissions:

```json
"permissions": [
  "storage",
  "activeTab",
  "identity",
  "https://your-api-domain.com/*"
]
```

> 🔒 These are kept minimal to ensure security.

---

## 🌐 API Integration

* **GET /profiles** – fetches all profiles user has access to.
* **POST /analysis** – sends selected profile and product details to the Analysis Service.

