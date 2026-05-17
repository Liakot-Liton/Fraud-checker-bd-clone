# Fraud-checker-bd 🇧🇩

An open-source, web-based fraud reporting, verification, and search platform designed to help individuals, consumers, and businesses identify scammers, fraudulent agents, or corrupt companies before entering a deal. 

The primary mission of this project is to prevent recurring fraud by mapping isolated scam incidents into unified, searchable identity profiles.

---

## 🚀 Key Features & Constraints Met

- **🔒 Separate User & Admin Paradigms:** Dedicated interfaces separate the public directory from the administrative verification terminal.
- **⚡ Unauthenticated Public Reporting:** Victims can quickly report fraud events, list losses, provide scam classifications, and append identification fields without needing to log in or create an account.
- **🛡️ Secure Administrative Moderation:** All incoming reports enter a protected, hidden holding queue. Only authenticated administrators can inspect, approve, or reject incidents.
- **🔄 Smart Identity Consolidation Engine:** When an incident is approved, the system automatically checks its phone numbers and unique identifiers against existing database structures. If a match is found, the incident is seamlessly merged into that culprit's existing "Cheater Profile" to build an immutable history.
- **🔍 Normalized Search Index:** Advanced text normalization strips non-alphanumeric characters, enabling high-accuracy searches by name, phone number, National ID (NID), or trade registration number.

---

## 🛠️ Technology Stack

To ensure that the project is accessible, lightweight, and highly maintainable for open-source developers, the first draft relies on a clean, zero-build ecosystem:

- **Runtime Environment:** Node.js
- **Backend Framework:** Express.js (REST API Endpoints)
- **Database Engine:** SQLite3 (Relational in-memory architecture for rapid prototype testing)
- **Frontend Architecture:** Clean HTML5, JavaScript (Fetch API), and utility-first responsive styling via Tailwind CSS CDN.

---

## 📂 Project Structure

```text
Fraud-checker-bd/
├── package.json              # Node.js project manifest and dependency tracker
├── server.js                 # Central Express app, REST routing, and SQLite schema
├── DEVELOPER_GUIDE.txt       # Local architectural blueprint and functional steps
├── README.md                 # Project manifesto and GitHub orientation (This file)
└── public/                   # Client-side user interface directory
    ├── index.html            # Public landing page, search engine, and profile browser
    ├── submit.html           # Public unauthenticated fraud incident reporting form
    └── admin.html            # Protected administrative authentication and moderation console
