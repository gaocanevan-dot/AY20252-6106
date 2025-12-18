# AY20252-6106

**Decentralized Financial Transaction DApp**

This repository contains the source code and supporting materials for the **SC6106 – Blockchain Development Fundamentals (Part 1)** group assignment. The project implements a decentralized financial transaction prototype that integrates a traditional web backend with Ethereum smart contracts, demonstrating core concepts of Web3-based application design.

---

## 📌 Project Overview

This project aims to explore how blockchain technology can be applied to basic financial transaction scenarios such as deposits and transfers. Traditional centralized systems often suffer from high transaction fees, limited transparency, and single points of failure. By introducing Ethereum smart contracts as a trusted execution layer, this application improves transparency, auditability, and trust without relying on centralized intermediaries.

The system adopts a hybrid **Web2 + Web3** architecture, combining a Flask backend for user interaction and logging with smart contracts deployed on a blockchain network for financial operations.

---

## 🧱 System Architecture

The application is composed of three main components:

* **Backend (Flask + SQLite)**
  Handles routing, page rendering, and lightweight user access logging. User visit records are stored locally in an SQLite database.

* **Frontend (HTML / CSS / JavaScript)**
  Provides a simple and responsive user interface for interacting with blockchain functions.

* **Blockchain Layer (Solidity + Web3.js)**
  Implements core financial logic using Ethereum smart contracts and enables client-side interaction via Web3.js.

---

## 🧩 Key Features

* Username-based user entry and navigation
* On-chain fund transfer and deposit functions
* Smart contract interaction via MetaMask and Web3.js
* Local user visit logging and log management
* Clear separation between on-chain immutable data and off-chain mutable records

---

## 🛠️ Technology Stack

* **Backend:** Python, Flask, SQLite
* **Frontend:** HTML, CSS, JavaScript
* **Blockchain:** Solidity, Ethereum (test network)
* **Web3 Integration:** Web3.js
* **Development Tools:** Remix IDE, MetaMask

---

## 📁 Project Structure

```
├── app.py                  # Main Flask application
├── user.db                 # SQLite database for user logs
├── requirements.txt        # Python dependencies
├── templates/              # HTML templates
│   ├── index.html
│   ├── main.html
│   ├── paynow.html
│   ├── deposit.html
│   ├── userlog.html
│   └── ...
├── static/
│   └── styles.css          # Frontend styles
└── README.md
```

---

## 🚀 Installation & Running

### 1. Clone the repository

```bash
git clone https://github.com/gaocanevan-dot/AY20252-6106.git
cd AY20252-6106
```

### 2. (Optional) Create a virtual environment

```bash
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the application

```bash
python app.py
```

The application will be available at:
`http://127.0.0.1:5000`

---

## 📖 Usage

1. Open the web application in your browser.
2. Enter a username on the welcome page.
3. Navigate to the main menu to access deposit or transfer functions.
4. Connect a Web3 wallet to perform blockchain transactions.
5. View or clear user access logs via the provided interfaces.

---

## ⚠️ Limitations

* The backend uses a global variable for session control, which may cause concurrency issues.
* No password-based authentication is implemented.
* Smart contract address and ABI are exposed in frontend source code.
* The project is intended for educational and demonstration purposes only.

---

## 🔮 Future Enhancements

* Introduce robust authentication mechanisms such as JWT or Flask-Login
* Replace SQLite with a production-grade database
* Improve UI feedback during blockchain transaction confirmation
* Enhance smart contract security and modularity

---

## 🎓 Learning Outcomes

Through this project, the team gained practical experience in:

* Smart contract design and Gas cost considerations
* Web3 client–contract interaction patterns
* Hybrid system architecture combining Web2 and Web3
* Differences between mutable off-chain data and immutable on-chain records

---

## 📄 License

This project is developed for academic coursework and does not include an explicit open-source license. Usage and modification are subject to course-related policies.

