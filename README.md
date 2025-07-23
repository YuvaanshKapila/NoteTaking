# NoteTaking App

A Firebase-backed web app built for fast and flexible note-taking directly in the browser.

## Features

- Real-time note creation and editing
- Persistent storage using Firebase Firestore
- Custom data connectivity via DataConnect
- Lightweight front-end powered by vanilla JavaScript and HTML

## File Overview

- `index.html` – Main web interface
- `firestore.rules` – Security rules for Firestore access
- `firestore.indexes.json` – Firestore indexing configuration
- `package.json` & `package-lock.json` – Project dependencies
- `dataconnect/` – Custom generated connector logic
- `firebase-debug.log` – Firebase diagnostic logging

## Setup Instructions

### Prerequisites

- Node.js and npm installed
- Firebase account and CLI installed

### Installation

1. Clone the repository:
git clone https://github.com/YuvaanshKapila/NoteTaking.git cd NoteTaking


2. Install dependencies:
npm install


3. Set up Firebase:
- Create a Firebase project
- Initialize Firebase in the project directory
- Replace SDK configs in `index.html` with your Firebase project's credentials
- Apply rules and indexes using:
  ```
  firebase deploy --only firestore:rules
  firebase deploy --only firestore:indexes
  ```

### Running the App Locally

You can preview `index.html` using a static file server like `live-server` or VS Code’s live preview.

### Firebase Hosting (Optional)

To deploy on Firebase Hosting:
firebase init hosting firebase deploy --only hosting


## License

MIT License. See `LICENSE` file if avail
