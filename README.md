# smart-medicine-reminder-
# Smart Medicine Reminder & Adherence Tracker

Stack: ESP32 firmware → Flask backend (SQLite) → React frontend → simple ML model

Quick start (local):
1. Backend:
   cd backend
   python3 -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   cp .env.example .env
   python db_init.py
   python app.py

2. Frontend:
   cd frontend
   npm install
   npm start

3. Firmware:
   Edit firmware/esp32_pillbox.ino (WIFI + SERVER_URL), upload to ESP32.

Ngrok (if using local device):
   ngrok http 5000
   set SERVER_URL to the ngrok https URL in firmware.
