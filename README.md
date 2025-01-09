# 🎶 Music Player Web Application 🎶

Welcome to the **Music Player Web Application**! This is a fully functional web-based music player that allows users to play and control a playlist of music tracks. The player supports multiple features like play/pause, skip next/previous, shuffle, repeat, and volume control. It offers a smooth and user-friendly interface to create a great listening experience.

---

## 📜 Table of Contents

- [Project Overview](#project-overview)

- [Features](#features)

- [Technologies Used](#technologies-used)

- [File Structure](#file-structure)

- [Installation](#installation)

- [Usage](#usage)

- [How It Works](#how-it-works)

- [Contributing](#contributing)

---

## 🎧 Project Overview

This **Music Player** is designed using **HTML5**, **CSS3**, and **JavaScript**. It's a client-side application that lets you manage and enjoy music tracks. The player features dynamic updates based on user actions, including playing and pausing music, skipping to the next or previous track, adjusting the volume, and toggling repeat and shuffle options.

The playlist is displayed on the side in a scrollable format, where each track shows an album cover and its metadata. The player is responsive, meaning it works seamlessly on both desktop and mobile devices.

---

## 🚀 Features

Here are the key features of this Music Player:

- **🎶 Dynamic Playlist**: Add multiple music tracks with album artwork and details.

- **⏯️ Play/Pause**: Toggle between playing and pausing the current song.

- **⏭️ Skip Next / ⏮️ Skip Previous**: Skip to the next or previous track in the playlist.

- **🔀 Shuffle**: Shuffle the tracks in a random order for a fun listening experience.

- **🔁 Repeat**: Repeat the current track indefinitely.

- **🔊 Volume Control**: Adjust the volume or mute the audio.

- **⏳ Track Progress**: Displays the current playtime and total duration of the song.

- **🎵 Playlist Toggle**: Open and close the playlist modal at will.

- **📱 Responsive Design**: Mobile-friendly and works well across devices.

---

## 🛠️ Technologies Used

This project was built using the following technologies:

- **HTML5**: Structure of the web page and audio player elements.

- **CSS3**: Styles and layout to create a modern, responsive interface.

- **JavaScript**: Logic for controlling the player and managing the music playlist.

- **Audio API**: To manage music playback, track progress, and control audio functions like play, pause, volume, and seek.

---

## 📂 File Structure

Here's the structure of the project:

```bash
📦 responsive-music-player

┣ 📂 css
┃ ┗ 📜 style.css          # Styles for the music player UI
┣ 📂 js
┃ ┗ 📜 script.js          # JavaScript for player functionality and controls
┃ ┗ 📜 music.js          # JavaScript for storing the songs details
┣ 📂 images
┃ ┗ 📜 poster-1.jpg        # Album posters
┃ ┗ 📜 poster-2.jpg
┣ 📂 music
┃ ┗ 📜 music-1.mp3          # Music files (add your own songs here)
┃ ┗ 📜 music-2.mp3
┗ 📜 index.html           # Main HTML file for the music player
```
---

### `music.js` Breakdown:

The `music.js` file contains:

- **🎶 Music Data**: An array of objects (`musicData`) that holds information about each track such as the title, artist, album, year, album cover URLs, and audio file path.

- **🖱️ Event Handlers**: Functions for managing user interactions like playing, pausing, skipping, adjusting volume, and changing the track.

- **🔄 DOM Manipulation**: Dynamically updates the player UI when a user interacts with the playlist or the player controls.

### `style.css` Breakdown:

The `style.css` file provides:

- **🎧 Player Controls**: Styling for buttons like play, pause, next, previous, shuffle, repeat, and volume control.

- **🎨 Playlist Design**: The playlist and individual tracks are styled to match the overall aesthetic.

- **📱 Responsive Design**: Ensures that the music player looks great on both desktop and mobile screens.

---

## ⚡ Installation

### 1. Clone the Repository

To get started, clone this repository to your local machine:

```bash
git clone https://github.com/your-username/music-player.git
```

### 2. Navigate to the Project Directory
```bash
cd music-player
```

### 3. Open index.html in Your Browser

Simply open the index.html file in your browser to run the Music Player. No need for a server-side setup as this is a static web app.

---

## 🕹️ Usage

Once the app is running, you can start interacting with the player. Here's how:

### 🎶 Music Controls:

- **⏯️ Play/Pause**: Click the play button to start the music. Click it again to pause the track.

- **⏭️ Next / ⏮️ Previous**: Use the next or previous buttons to skip through the playlist.

- **🔀 Shuffle**: Toggle the shuffle button to randomize the playlist order.

- **🔁 Repeat**: Click the repeat button to loop the current track.

- **🔊 Volume**: Adjust the volume slider to change the sound level or click the speaker icon to mute.

- **⏳ Track Progress**: Drag the seek bar to move forward or backward within the track.

### 📑 Playlist Interaction:

- Click on any track in the playlist to switch to that song.

- The currently playing track will be highlighted with a special visual indicator.

### 🎧 Toggle Playlist Modal:

- Use the playlist icon button to open or close the playlist sidebar for easy navigation.

---

## ⚙️ How It Works

### 1. **Music Data**:

The `music.js` file contains an array of objects (`musicData`). Each object represents a music track and holds the following properties:

- `backgroundImage`: URL of the background image to be displayed while the music plays.

- `posterUrl`: Album cover image URL.

- `title`: Name of the track.

- `album`: The album the track belongs to.

- `year`: Release year.

- `artist`: Artist performing the song.

- `musicPath`: Path to the MP3 file.

### 2. **Audio Playback**:
When a user clicks a song, the **Audio API** is used to load the track and start playback. The player dynamically updates to reflect the song's title, artist, album, and cover art.

### 3. **Player Controls**:

- **⏯️ Play/Pause**: Controls the audio element to toggle between playing and paused states.

- **⏭️ Skip Next / ⏮️ Skip Previous**: Navigates through the playlist, updating the UI with the new track.

- **🔀 Shuffle**: Randomizes the current playlist order.

- **🔁 Repeat**: Loops the current song if activated.

- **🔊 Volume Control**: Adjust the volume or mute/unmute the player.

### 4. **Playlist Modal**:
The playlist is accessible through a toggle button that opens and closes a modal, displaying the available tracks. Clicking on a song will update the player to play the selected track.

---

## 🤝 Contributing

We welcome contributions to improve this project! If you'd like to contribute, follow these steps:

### 1. Fork the repository.

### 2. Create a new branch: 
```bash
git checkout -b feature-name.
```


### 3. Make your changes and commit them: 
```bash
git commit -am 'Add new feature'.
```

### 4. Push to your branch: 
```bash
git push origin feature-name.
```

### 5. Open a pull request on GitHub.

---

## Future Enhancements:-

- Song Search Feature: Add a search bar to quickly find songs within the playlist.

- Theme Customization: Add options for users to switch between light and dark modes.

- Lyrics Display: Implement a feature to display lyrics alongside the song.

- Offline Support: Add support for playing songs offline using service workers.
