# 🎬 Movie Night: Watch Together

![Movie Night Logo](/public/images/Life%20Logo.png)

Movie Night is a real-time collaborative movie-watching platform that allows you and your friends to sync video playback, chat, and react together, no matter where you are. Built with modern web technologies and powered by Firebase, it offers a seamless and interactive experience for shared entertainment.

## ✨ Features

*   **Real-time Video Synchronization:** Watch movies together with perfectly synchronized playback across all participants.
*   **Collaborative Play/Pause:** Any connected user can pause or play the video, and the action is instantly synchronized for everyone.
*   **Host-Only Seeking:** The room host maintains control over skipping forward/backward in the video, ensuring smooth transitions.
*   **Dynamic Floating Chat:** A draggable and resizable chat window that stays visible even when the video is in full-screen mode, allowing continuous interaction.
*   **Mobile Chat Overlay:** On smaller screens, the chat transforms into a full-screen overlay for an optimized mobile experience.
*   **Live User Presence:** See who's online and their current player status (playing/paused) in real-time.
*   **In-Chat Movie Timestamps:** Messages include the movie's playback time at the moment they were sent, providing context for discussions.
*   **Typing Indicators:** See when others are typing in the chat.
*   **Expressive Reactions:** Send animated emoji reactions that appear on the video screen.
*   **Room Management:** Create private rooms with custom names, descriptions, and participant limits.
*   **Movie Search & Selection:** Easily search for movies and select quality options from integrated APIs.
*   **Manual Movie URL Input:** Option to manually enter a direct video URL if you have one.
*   **Room Sharing:** Share room links and IDs via various platforms (WhatsApp, Telegram, Email) or QR code.
*   **User Authentication:** Secure login and registration powered by Firebase Authentication.
*   **Responsive Design:** Optimized for both desktop and mobile devices.

## 🚀 Getting Started

To run this project locally, you'll need to set up a Firebase project and configure its services.

1.  **Clone the repository:**
    \`\`\`bash
    git clone <your-repo-url>
    cd movie-night
    \`\`\`
2.  **Set up Firebase:**
    *   Go to the [Firebase Console](https://console.firebase.google.com/).
    *   Create a new project.
    *   Add a web app to your Firebase project.
    *   Copy your Firebase configuration object (apiKey, authDomain, projectId, etc.).
    *   Update the `firebaseConfig` object in `login.html`, `register.html`, and `index.html`, and `room.html` with your project's details.
    *   **Enable Firebase services:**
        *   **Authentication:** Go to "Authentication" -> "Sign-in method" and enable "Email/Password".
        *   **Firestore Database:** Create a Firestore database in "production mode".
        *   **Realtime Database:** Create a Realtime Database.
    *   **Deploy Firestore Security Rules:** Copy the content from `firestore.rules` into your Firestore "Rules" tab and publish.
    *   **Deploy Realtime Database Rules:** Copy the content from `database.rules.json` into your Realtime Database "Rules" tab and publish.
    *   **Create Firestore Composite Index:** For the "My Rooms" section to load efficiently, you might need a composite index for `rooms` collection on `creator.uid` (Ascending) and `createdAt` (Descending). Firebase will usually suggest this in the console if needed.

3.  **Run the application:**
    Since this is a client-side application with HTML, CSS, and JavaScript, you can simply open the `login.html` file in your web browser. For a more robust local development experience, you can use a simple local web server (e.g., `npx serve` or Python's `http.server`).

    \`\`\`bash
    # Using npx serve (if you have Node.js installed)
    npx serve .
    \`\`\`
    Then, open your browser to `http://localhost:3000/login.html` (or the port `serve` indicates).

## 🎥 Demo

![Movie Night GIF](/public/images/movie.gif)

## 🤝 Contribution

This project is open-source and created for the community. Feel free to fork, contribute, and improve!

---

**Developed By Kawdhitha Nirmal And Member Of Cyber Yakku TM**
**Created For Community**
