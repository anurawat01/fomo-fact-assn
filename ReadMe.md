----
# Crypto/Stock Real-Time Update Mini Website

Welcome to the mini website for real-time crypto and stock updates!

## Overview

This project pulls real-time cryptocurrency information from CoinGecko using their API. Due to the limitations of the free version of the API (30 calls per minute), the application refreshes every 60 seconds. The refresh rate is displayed on the UI.

### Backend Configuration

- **Environment Variables**: 
  - MongoDB URL
  - CoinGecko API key
  - Note: For security reasons, environment variables are not included in the code. Ideally, AWS Secrets Manager or a similar service should be used to manage these secrets, but due to time constraints, this was not implemented.

### Running the Application

1. **Frontend**:
   - Navigate to the `frontend` directory in your terminal.
   - Run the command:
     ```bash
     npm start
     ```
   - The frontend will be served on port 3000 by default.

2. **Backend**:
   - Navigate to the `backend` directory in your terminal.
   - Run the command:
     ```bash
     npx ts-node-dev src/app.ts
     ```
   - The backend will also run on port 3000 by default, but you can change the port if needed.

### Usage

- By default, the UI will display Bitcoin (BTC) details.
- You can change the cryptocurrency symbol using the input box provided. The supported symbols are listed in the yellow box on the UI.

### Contact

If you encounter any issues or have questions, please feel free to reach out to me at: [anubhavrawat62@gmail.com](mailto:anubhavrawat62@gmail.com).

---

Feel free to tweak any part of this to better fit your needs or style!