# 🎵 Premium Music Player

A stunning Windows desktop music player application built with Electron, featuring system tray integration, audio visualization, mini player mode, and a modern, premium UI with full Windows OS integration.

![Music Player](assets/icon.png)

## ✨ Features

### 🎵 **Audio Playback**
- Full playback controls (Play, Pause, Stop, Next, Previous)
- Seek functionality with progress bar
- Volume control with mute option
- Support for multiple audio formats (MP3, WAV, OGG, FLAC, M4A, AAC, WMA)
- Seamless track transitions

### 🎨 **Beautiful Interface**
- Modern, premium design with smooth animations
- Dark and Light theme support
- Custom title bar with window controls
- Glassmorphic effects and vibrant gradients
- Responsive layout
- Mini player mode for compact playback

### 📊 **Audio Visualizer**
- Real-time audio spectrum analyzer
- Beautiful gradient visualization
- Synced with audio playback

### 📋 **Playlist Management**
- Create and manage playlists
- Add songs from files or folders
- Queue management
- Reorder tracks (drag & drop coming soon)

### 🔀 **Playback Modes**
- **Shuffle**: Random playback order
- **Repeat**: Off / Repeat All / Repeat One
- Seamless track transitions

### 🔍 **Search & Browse**
- Search songs by title, artist, or album
- Browse your entire music library
- View current queue

### 🪟 **Windows OS Integration**
- **File Associations**: Set as default app for music files (.mp3, .wav, .flac, .m4a, .aac, .ogg)
- **Program Files Installation**: Proper installation to Program Files directory
- **Start Menu Integration**: Shortcuts in Start Menu under "Music" category
- **Desktop Shortcut**: Optional desktop shortcut during installation
- **Programs and Features**: Appears in Windows "Add or Remove Programs"
- **Uninstaller**: Complete uninstallation with registry cleanup
- **Context Menu**: "Open With" integration for music files
- **Double-click Support**: Open music files directly from Windows Explorer

### 🎛️ **System Tray Integration**
- Minimize to system tray
- Continue playing in background
- Quick controls from tray menu (Play/Pause, Next, Previous, Quit)
- Tray icon with tooltip showing current track
- Double-click tray icon to restore window
- Background playback notifications

### 💾 **Persistent Settings**
- Remembers your music library
- Saves volume and playback preferences
- Retains theme selection
- Stores playlists
- Window size and position memory

## 🚀 Getting Started

### For End Users

**Download & Install:**

1. Download `Premium Music Player-Setup-1.0.5.exe` from releases
2. Run the installer
3. Choose installation location (default: `C:\Program Files\Premium Music Player`)
4. Select additional options:
   - Desktop shortcut
   - Start Menu shortcut
5. Click Install and wait for completion
6. Launch the application

**Features After Installation:**
- Music files automatically associated with Premium Music Player
- Set as default app for music files in Windows Settings
- Access from Start Menu → All Apps → Music → Premium Music Player
- Right-click any music file → "Open with Premium Music Player"
- Uninstall via Windows Settings → Apps → Premium Music Player



## 🎯 Usage

### Installing the Application

1. **Run the Installer**: Double-click `Premium Music Player-Setup-1.0.0.exe`
2. **Choose Options**: Select installation directory and shortcuts
3. **Complete Installation**: Wait for the process to finish
4. **Launch**: Click "Finish" to launch immediately or find it in Start Menu

### Adding Music

1. **Add Files**: Click the "Add Files" button or use the file icon in the top bar
2. **Add Folder**: Click the "Add Folder" button to import an entire music folder
3. **Open from Explorer**: Right-click any music file → "Open with Premium Music Player"
4. **Double-click**: After setting as default, double-click music files to open

### Playing Music

1. Click any song in your library to start playing
2. Use the player controls at the bottom
3. Adjust volume with the slider
4. Enable shuffle or repeat modes as desired
5. Switch to mini player for compact playback

### Creating Playlists

1. Click "Create Playlist" in the sidebar
2. Enter a name for your playlist
3. Add songs to the playlist from your library

### System Tray

- Click the **X** button to minimize to tray (doesn't close the app)
- Music continues playing in the background
- Right-click the tray icon for quick controls:
  - Show App
  - Play/Pause
  - Next Track
  - Previous Track
  - Quit
- Double-click the tray icon to restore the window

### Setting as Default Music Player

**Windows 10/11:**
1. Right-click any music file (.mp3, .flac, etc.)
2. Select "Open with" → "Choose another app"
3. Select "Premium Music Player"
4. Check "Always use this app to open .mp3 files"
5. Click OK

**Or via Windows Settings:**
1. Open Settings → Apps → Default apps
2. Scroll to "Music Player"
3. Select "Premium Music Player"

## 🎨 Themes

Toggle between Dark and Light themes using the theme button in the sidebar.

- **Dark Theme**: Perfect for nighttime listening with vibrant accents
- **Light Theme**: Clean and modern for daytime use

## 🔧 Technical Details

### Built With
- **Electron v28**: Desktop application framework
- **HTML/CSS/JavaScript**: Core web technologies
- **Web Audio API**: Audio visualization and processing
- **LocalStorage**: Settings persistence
- **NSIS**: Windows installer creation
- **electron-builder**: Build and packaging tool

### System Requirements
- **OS**: Windows 10/11 (64-bit)
- **RAM**: 256 MB minimum
- **Disk Space**: 100 MB for installation
- **Audio**: Windows-compatible audio device

### Audio Formats Supported
- **MP3** (.mp3) - MPEG Audio Layer 3
- **WAV** (.wav) - Waveform Audio File
- **OGG** (.ogg) - Ogg Vorbis
- **FLAC** (.flac) - Free Lossless Audio Codec
- **M4A** (.m4a) - MPEG-4 Audio
- **AAC** (.aac) - Advanced Audio Coding
- **WMA** (.wma) - Windows Media Audio

### Installation Details
- **Install Location**: `C:\Program Files\Premium Music Player\` (default)
- **Uninstaller**: `C:\Program Files\Premium Music Player\Uninstall Premium Music Player.exe`
- **Registry**: HKCU\Software\Classes (file associations)
- **Start Menu**: Start Menu\Programs\Music\Premium Music Player
- **AppData**: Settings stored in `%APPDATA%\premium-music-player\`

### File Associations
The installer automatically registers the following extensions:
- `.mp3`, `.wav`, `.flac`, `.m4a`, `.aac`, `.ogg`
- Appears in "Open With" context menu
- Can be set as default application for each format

## 🐛 Troubleshooting

### Installation Issues

**"Windows protected your PC" message:**
- This is normal for unsigned applications
- Click "More info" → "Run anyway"
- Consider code signing for production distribution

**Installation fails or requires admin:**
- Right-click installer → "Run as administrator"
- Or choose a user-writable directory during installation

### Audio Issues

**Audio not playing:**
- Check that the file format is supported
- Ensure the file path is accessible
- Verify Windows audio is working
- Try restarting the application
- Check volume isn't muted in app or Windows

**Visualizer not working:**
- The visualizer requires an active audio context
- Click play on a song to initialize the visualizer

### System Tray Issues

**Tray icon not appearing:**
- Check Windows notification area settings
- Right-click taskbar → Taskbar settings → Select which icons appear
- Enable "Premium Music Player"
- Ensure the app has permission to run in the background

**Can't restore from tray:**
- Double-click the tray icon
- Or right-click → "Show App"
- If stuck, End the Task for the App via Task Manager

### File Association Issues

**Music files don't open with the app:**
- Right-click file → Properties → Change → Select Premium Music Player
- Or reinstall the application
- Check Windows default apps settings

**"Open With" doesn't show the app:**
- Reinstall to re-register file associations
- Manually browse to: `C:\Program Files\Premium Music Player\Premium Music Player.exe`

### Uninstallation Issues

**Can't find uninstaller:**
- Windows Settings → Apps → Premium Music Player → Uninstall
- Or run: `C:\Program Files\Premium Music Player\Uninstall Premium Music Player.exe`
- Manual removal: Delete installation folder + registry keys

**Files remain after uninstall:**
- User data is intentionally preserved in `%APPDATA%`
- Manually delete `%APPDATA%\premium-music-player\` if desired

## 🚧 Future Enhancements

- [ ] Drag & drop file support
- [ ] Album artwork extraction from metadata
- [x] Equalizer controls
- [ ] Lyrics display
- [ ] Last.fm scrobbling
- [ ] Import/Export playlists (M3U, PLS)
- [ ] Discord Rich Presence
- [x] Cross-fade between tracks
- [ ] Sleep timer
- [ ] Audio normalization
- [ ] Podcasts support
- [ ] Internet radio streams
- [x] Auto-update functionality
- [ ] Cloud sync for playlists
- [ ] Keyboard media key customization

## ✅ Completed Features

- [x] Mini player mode
- [x] System tray integration
- [x] Windows OS integration (file associations, installer, uninstaller)
- [x] Program Files installation
- [x] Dark/Light themes
- [x] Audio visualization
- [x] Keyboard shortcuts
- [x] Global media key support
- [x] Playlist management
- [x] Search functionality
- [x] Shuffle and repeat modes

## 📦 Distribution

### For End Users
Download the installer from the releases page and run it. The installer handles everything:
- Installation to Program Files
- File associations registration
- Start Menu shortcuts
- Desktop shortcuts
- System integration

## 🙏 Acknowledgments

- Icons and design inspired by modern music players
- Built with love for music enthusiasts
- Thanks to the Electron community for excellent documentation
- Web Audio API for powerful audio processing capabilities
- NSIS for reliable Windows installer creation

## 📊 Project Stats

- **Language**: JavaScript, HTML, CSS
- **Framework**: Electron 28
- **Installer**: NSIS
- **Build Tool**: electron-builder
- **Target Platform**: Windows 10/11 (64-bit)
- **Package Size**: ~73 MB (includes Electron runtime)

---

**If you find this project helpful, you can support my work here:**

<p align="center">
  <a href="https://www.buymeacoffee.com/rondinabrybry" target="_blank" rel="noopener noreferrer">
    <img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" />
  </a>
</p>

**Enjoy your music! 🎵**

*Premium Music Player - A modern, feature-rich music player for Windows*
