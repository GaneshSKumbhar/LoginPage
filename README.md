# Notes App with Firebase Authentication

A simple web-based Notes App that allows users to log in via email/password or Google authentication using Firebase. After logging in, users are redirected to a dashboard where they can view sample notes.

## Features

- **User Authentication**: Supports email/password sign-up and login, as well as Google sign-in.
- **Secure Login**: Integrated with Firebase Authentication for secure user management.
- **Dashboard**: Post-login dashboard displaying sample notes with a clean, responsive UI.
- **Logout Functionality**: Users can log out and return to the login page.
- **Responsive Design**: Modern UI with gradient backgrounds and hover effects.

## Technologies Used

- **HTML5**: Structure of the web pages.
- **CSS3**: Styling for a modern, responsive design.
- **JavaScript (ES6 Modules)**: Client-side logic for authentication and interactions.
- **Firebase**: Authentication service for user login and sign-up.

## Prerequisites

- A web browser (e.g., Chrome, Firefox).
- Internet connection for Firebase services.
- A Firebase project set up (see Setup section).

## Setup Instructions

1. **Clone or Download the Project**:
   - Download the project files (`login.html`, `dashboard.html`, `README.md`) to your local machine.

2. **Set Up Firebase Project**:
   - Go to the [Firebase Console](https://console.firebase.google.com/).
   - Create a new project or use an existing one.
   - Enable Authentication:
     - In the Firebase Console, navigate to Authentication > Sign-in method.
     - Enable Email/Password and Google providers.
   - Get your Firebase configuration:
     - Go to Project Settings > General > Your apps.
     - If no app is added, click "Add app" and select Web.
     - Copy the Firebase config object (apiKey, authDomain, etc.).

3. **Configure Firebase in the Code**:
   - Open `login.html` and `dashboard.html` in a text editor.
   - Replace the `firebaseConfig` object with your own Firebase configuration:
     ```javascript
     const firebaseConfig = {
       apiKey: "YOUR_API_KEY",
       authDomain: "YOUR_AUTH_DOMAIN",
       projectId: "YOUR_PROJECT_ID",
       storageBucket: "YOUR_STORAGE_BUCKET",
       messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
       appId: "YOUR_APP_ID",
       measurementId: "YOUR_MEASUREMENT_ID"
     };
     ```
   - Save the files.

4. **Run the Application**:
   - Open `login.html` in your web browser.
   - The app will load and allow users to sign up or log in.

## Screenshots

### Login Page
![Login Page](![alt text](image.png))
*Description: The login page with email/password fields and Google sign-in option.*

### Dashboard
![Dashboard](![alt text](image-1.png))
*Description: The dashboard displaying sample notes after successful login.*

## Usage

1. **Login/Sign Up**:
   - Open `login.html` in your browser.
   - Enter your email and password, then click "Sign Up" to create an account or "Login" to sign in.
   - Alternatively, click "Sign in with Google" to authenticate via Google.

2. **Dashboard**:
   - After successful authentication, you'll be redirected to `dashboard.html`.
   - View the welcome message with your name/email.
   - See sample notes displayed in cards.
   - Click "Logout" to sign out and return to the login page.

## Project Structure

- `login.html`: The login page with authentication forms.
- `dashboard.html`: The dashboard page for logged-in users.
- `README.md`: This documentation file.

## Contributing

Feel free to fork the project and submit pull requests for improvements.

## License

This project is open-source and available under the MIT License.
