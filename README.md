# 🌱 Smart-Farming Agent

An AI-powered smart farming assistant built with **IBM watsonx Orchestrate**, embedded as a web chat widget for real-time agricultural guidance.

---

## 📖 Overview

The **Smart-Farming Agent** is an intelligent conversational agent designed to assist farmers and agri-businesses with:

- Crop management recommendations
- Soil health and irrigation advice
- Weather-based farming decisions
- Pest and disease identification
- Yield optimization strategies

The agent is deployed via **IBM watsonx Orchestrate** and embedded directly into a lightweight HTML page using the `wxoLoader` script.

---

## 🚀 Features

- ✅ AI chat interface powered by IBM watsonx Orchestrate
- ✅ Embedded web widget — no complex frontend framework required
- ✅ Responsive and mobile-friendly layout
- ✅ Easy to deploy on any static hosting platform (GitHub Pages, Netlify, Vercel, etc.)

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 | Page structure |
| IBM watsonx Orchestrate | AI agent backend |
| `wxoLoader.js` | Chat widget loader |

---

## 📁 Project Structure

```
smart-farming-agent/
│
├── index.html        # Main entry point with embedded chat agent
└── README.md         # Project documentation
```

---

## ⚙️ Setup & Configuration

### 1. Clone the repository

```bash
git clone https://github.com/your-username/smart-farming-agent.git
cd smart-farming-agent
```

### 2. Configure your IBM watsonx Orchestrate credentials

Open `index.html` and update the `wxOConfiguration` object with your own credentials:

```javascript
window.wxOConfiguration = {
  orchestrationID: "YOUR_ORCHESTRATION_ID",
  hostURL: "https://your-region.watson-orchestrate.cloud.ibm.com",
  rootElementID: "root",
  deploymentPlatform: "ibmcloud",
  crn: "YOUR_CRN",
  chatOptions: {
    agentId: "YOUR_AGENT_ID",
    agentEnvironmentId: "YOUR_ENVIRONMENT_ID",
  }
};
```

### 3. Open in browser

Simply open `index.html` in any modern browser — no build step required.

```bash
# Or serve locally with Python
python -m http.server 8080
```

Then navigate to `http://localhost:8080`.

---

## 🌐 Deployment

### GitHub Pages

1. Push your code to a GitHub repository.
2. Go to **Settings → Pages**.
3. Set the source to your main branch and root folder.
4. Your agent will be live at `https://your-username.github.io/smart-farming-agent/`.

### Netlify / Vercel

Drag and drop the project folder into [Netlify Drop](https://app.netlify.com/drop) or connect your GitHub repo to Vercel for instant deployment.

---

## 🔐 IBM watsonx Orchestrate Setup

To use this agent you need an active **IBM watsonx Orchestrate** instance. Follow the official IBM documentation to:

1. Create a watsonx Orchestrate environment on [IBM Cloud](https://cloud.ibm.com).
2. Build and publish your agent.
3. Copy your `orchestrationID`, `agentId`, `agentEnvironmentId`, and `CRN` into `index.html`.

---

## 📸 Screenshot

> _Add a screenshot of your deployed agent here._

```
![Smart-Farming Agent Screenshot](screenshot.png)
```

---

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

1. Fork the repository
2. Create a new branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m "Add your feature"`
4. Push to the branch: `git push origin feature/your-feature`
5. Open a Pull Request

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 👤 Author

**Your Name**
- GitHub: [saihitesh1448](https://github.com/saihitesh1448)
- LinkedIn: [Kamma Hitesh](https://www.linkedin.com/in/kamma-hitesh-65a5b137b/)

---

> _Built with ❤️ for smarter, sustainable farming._
