#kid-safety-watch-backend

# KidSafetyWatch Backend

Backend for the KidSafetyWatch app, built with Node.js, Express, Firebase Functions, and Firestore on Google Cloud Platform.

## Features

- REST API for health data storage and retrieval
- Ready for deployment to Firebase Functions or Google Cloud Run

## Setup

1. Install Firebase CLI:
   ```sh
   npm install -g firebase-tools
   ```

2. Initialize and login:
   ```sh
   firebase login
   firebase init
   ```

3. Install dependencies:
   ```sh
   cd functions
   npm install
   ```

4. Deploy:
   ```sh
   firebase deploy --only functions
   ```

## API Endpoints

- `POST /health-data` — Store new health data
- `GET /health-data/:userId` — Retrieve health data for a user

---
