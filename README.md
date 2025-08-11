# Feedback & Error Report Web App

A simple, modern feedback form for collecting bug reports, suggestions, and user feedback. Submissions are sent to both a Google Apps Script endpoint (for email notifications) and a Firebase Realtime Database (for storage).

## Features
- Responsive, mobile-friendly UI with Inter font
- Client-side validation for name and email
- Accepts any mobile number format
- Modal dialog for feedback status
- Submits feedback to:
  - Google Apps Script (email notification)
  - Firebase Realtime Database (data storage)

## Technologies Used
- HTML, CSS, JavaScript
- Google Apps Script (backend email notification)
- Firebase Realtime Database (client-side data storage)

## Firebase Database Rules Example
To allow writes but restrict reads:
```json
{
  "rules": {
    ".read": false,
    ".write": true
  }
}
```

## Customization
- Change the logo by replacing `logo.png`.
- Edit form fields or styles in `index.html` as needed.

## Security Notes
- The Firebase config is public and intended for client-side use. For sensitive data, use server-side validation and authentication.
- The Apps Script endpoint should validate and sanitize all input.