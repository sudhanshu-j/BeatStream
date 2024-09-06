# 🎶 Responsive Music Player 🎶

Overview:-

    This Responsive Music Player is a full-featured web application built using HTML, CSS, and JavaScript. It comes with 
    essential functionalities such as playlists, shuffle, repeat, and volume controls, along with a modern user interface. 
    It also displays song details such as name, artist, album, and album art.

Features:-

    • Play/Pause: Play or pause the current track.

    • Next/Previous: Skip to the next or previous track.

    • Shuffle: Randomize the order of the songs in the playlist.

    • Repeat: Repeat the current track once it ends.

    • Playlist Section: View and select from a list of available songs.

    • Song Details Display: Shows song title, artist, album, and poster artwork on the screen.

    • Volume Control: Adjust the volume using a slider for precise control.

    • Progress Bar: Shows the playback progress and allows you to seek by clicking or dragging.

    • Responsive Design: Fully responsive layout that works across mobile, tablet, and desktop devices.

Technologies Used:-

    • HTML: Structuring the elements and layout of the music player.

    • CSS: Styling the UI with a focus on responsiveness and modern design.

    • JavaScript: Handling the functionality for music control, playlist management, and DOM manipulation.

Getting Started:-

    Prerequisites

      To run this music player locally, all you need is a modern web browser.

    Installation

      1. Clone the repository:

        git clone https://github.com/yourusername/responsive-music-player.git

      2. Navigate to the project directory:

        cd responsive-music-player

      3. Open the index.html file in your browser:

         open index.html

Usage:-

    • Play/Pause: Click the play button to start playing music and the same button to pause.

    • Next/Previous: Use the next and previous buttons to switch between songs.

    • Shuffle: Toggle the shuffle button to randomize the playback order.

    • Repeat: Toggle the repeat button to repeat the current song once it ends.

    • Playlist: Select a song from the playlist section to start playing it.

    • Volume: Adjust the volume with the volume slider.

    • Progress Bar: Track progress with the bar, and click or drag to skip to different parts of the song.

Adding Your Own Music:-

    1. Add your songs to the music file.

    2. Update the playlist in music.js with the new song information (e.g., title, artist, album, poster image):

    const musicData = [
    {
      backgroundImage: "./assets/images/poster-1.jpg",
      posterUrl: "./assets/images/poster-1.jpg",
      title: "Aayi Nai - Stree 2 ",
      album: "Stree 2",
      year: 2024,
      artist: "Pawan Singh",
      musicPath: "./assets/music/music-1.mp3",
    },

    ]

Project Structure:-

    📦 responsive-music-player
    ┣ 📂 assets/
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

Code Snippets:- 

"NOTE:- ALL THIS CODE ARE RANDOM IT IS NOT INCLUDED IN THE ORIGINAL FILE"

HTML:-

    <div class="player">
      <div class="song-info">
    <img src="img/poster1.jpg" id="poster" alt="Album Art">
    <h2 id="title">Song Title</h2>
    <p id="artist">Artist Name</p>
    <p id="album">Album Name</p>
    </div>

    <audio id="audio"></audio>
  
    <div class="controls">
    <button id="prev">⏮️</button>
    <button id="play">▶️</button>
    <button id="next">⏭️</button>
    <button id="shuffle">🔀</button>
    <button id="repeat">🔁</button>
    </div>

    <input type="range" id="progress-bar" value="0" max="100">
    <input type="range" id="volume-slider" min="0" max="1" step="0.1" value="1">

    <div class="playlist">
    <ul id="playlist">
      <li>Song Title 1 - Artist 1</li>
      <li>Song Title 2 - Artist 2</li>
    </ul>
    </div>
    </div>

CSS:-

    .song-info {
     text-align: center;
    }

    .controls {
     display: flex;
     justify-content: center;
     gap: 15px;
    }

    #progress-bar, #volume-slider {
      width: 100%;
    }

    .playlist {
      margin-top: 20px;
    }

JavaScript:-

    const audio = document.getElementById('audio');
    const playBtn = document.getElementById('play');
    const prevBtn = document.getElementById('prev');
    const nextBtn = document.getElementById('next');
    const shuffleBtn = document.getElementById('shuffle');
    const repeatBtn = document.getElementById('repeat');
    const progressBar = document.getElementById('progress-bar');
    const volumeSlider = document.getElementById('volume-slider');
    const playlist = document.getElementById('playlist');

    let songs = [
    {
    name: 'Song Title 1',
    artist: 'Artist 1',
    album: 'Album 1',
    poster: 'img/poster1.jpg',
    file: 'music/song1.mp3'
    },
    {
    name: 'Song Title 2',
    artist: 'Artist 2',
    album: 'Album 2',
    poster: 'img/poster2.jpg',
    file: 'music/song2.mp3'
    }
  
    ];

    let currentSongIndex = 0;
    let isShuffle = false;
    let isRepeat = false;

    // Logic for playing, shuffling, repeating songs

Future Enhancements:-

    • Song Search Feature: Add a search bar to quickly find songs within the playlist.

    • Theme Customization: Add options for users to switch between light and dark modes.

    • Lyrics Display: Implement a feature to display lyrics alongside the song.

    • Offline Support: Add support for playing songs offline using service workers.






