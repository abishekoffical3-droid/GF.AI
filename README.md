# PRIYA AI v2 ULTRA — Abishek's Project

## What this ZIP contains
A substantially upgraded Android + Node.js starter project for PRIYA AI.

### Android
- Animated futuristic home screen
- Voice input using Android speech recognition
- Text chat
- Text-to-speech playback for PRIYA replies
- Owner profile field (default: Abishek Bhusal)
- Nepali / English / Hindi-ready interaction
- Secure architecture: Android never contains the Gemini API key

### Backend
- Express proxy for Gemini
- `.env` secret storage
- Helmet security headers
- Rate limiting
- Request-size limits
- Configurable CORS
- Configurable model name

## Important security note
The API key previously shared in chat should be treated as exposed. Revoke/rotate it and use a newly created key in `backend/.env` only.

## Setup
### Backend
1. `cd backend`
2. `cp .env.example .env`
3. Put a NEW Gemini key into `.env`
4. `npm install`
5. `npm start`

### Android Studio
Open the project root in Android Studio, allow Gradle sync, then run on your phone/emulator.
In PRIYA Settings, set your deployed backend URL. For local testing, Android emulator and real phones require different localhost/network addresses.

## Honest status
This is a strong source-code foundation, not a claim of universal 100% bug-free compatibility. Build/test on your exact Android Studio + device, then fix any environment-specific errors.

## Next upgrade ideas
- DataStore encrypted settings
- Real persistent user-approved memory
- Camera/image understanding through backend
- PDF/document upload and summarization
- Wake word/hands-free mode
- Web search via a server-side provider
- Authentication and per-user accounts
