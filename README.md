# Coffee Loyalty QR Scanner

This project implements a coffee loyalty system where users scan unique coffee shop QR codes to register their coffee purchases. On the 5th coffee, users get a free coffee confirmation email.

## How to Run

### Backend

1. Navigate to `backend` folder:

2. Install dependencies:

3. Edit `server.js` to set your Gmail and app password in the Nodemailer transporter section.

4. Start backend server:

### Frontend

1. Open a new terminal and navigate to `frontend` folder:

2. Install dependencies:

3. Start React app:

4. Open `http://localhost:3000` in your browser.

## Usage

- Enter your email.
- Click "Start Scan" to allow camera access.
- Scan the coffee shop's QR code (which should encode a JSON with the shopId, e.g. `{"shopId":"brand1-location1"}`).
- Your scans will be recorded.
- After 4 unique scan days, you get a popup with a free coffee confirmation.
- Click "Send Email Confirmation" to get an email with your coffee history.

## Notes

- For production, replace JSON file storage with a proper database.
- Use a Gmail App Password or OAuth2 for secure email sending.
- QR codes can be generated using any QR code tool that encodes JSON strings with a `shopId` field.

Enjoy your coffee loyalty app! ☕🎉
