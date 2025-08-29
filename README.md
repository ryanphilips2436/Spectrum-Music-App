# 🎶 Spectrum Music  

**Spectrum Music** is a desktop music player built with **Python**, combining a modern **CustomTkinter GUI**, **Pygame for audio playback**, **MySQL database integration**, and a **real-time audio visualizer** powered by **PyAudio + FFT analysis**.  

---

## ✨ Features  
- 🔑 **User Authentication** – Secure login and signup system (MySQL backend).  
- 🎵 **Music Playback** – Play, pause, stop, skip songs with Pygame mixer.  
- 📂 **Playlist Management** – Create and manage playlists, stored in MySQL.  
- 🖼️ **Interactive UI** – Built with CustomTkinter for a modern, clean look.  
- 📧 **Email Integration** – Sends confirmation emails on signup/login.  
- 📊 **Music Visualizer** – Real-time **frequency spectrum analyzer** using PyAudio and FFT (Fast Fourier Transform).  
- 🛠️ **Error Handling** – Handles missing files, invalid logins, and database errors gracefully.  

---

## 🏗️ Tech Stack  
- **Python 3.12**  
- **Pygame** (for audio playback)  
- **CustomTkinter** (for modern UI)  
- **MySQL** (for database storage)  
- **PIL (Pillow)** (for image handling)  
- **smtplib** (for email notifications)  
- **PyAudio + NumPy** (for real-time FFT audio visualization)  

---

## ⚠️ Important Notes (Before Running)  

1. 📦 **Modules Installation**  
   - All required modules must be installed using `pip`:  
     ```bash
     pip install pygame customtkinter pillow mysql-connector-python pyaudio numpy
     ```

2. 🗄️ **MySQL Database Setup**  
   - Import the provided `spectrum.sql` file into your MySQL server:  
     ```bash
     mysql -u root -p spectrum < spectrum.sql
     ```
   - Make sure your MySQL server is running and accessible.

3. 🌐 **API Setup**  
   - The project uses APIs (originally via RapidAPI).  
   - **You must create your own API key** and update it in the code.  
   - Example: Replace the placeholder API key with your own key from RapidAPI.  
   - Additionally, integrate a **Spotify API** for fetching track/artist metadata.  
     - Create a Spotify developer account here: [Spotify for Developers](https://developer.spotify.com/dashboard/)  
     - Generate your **Client ID** and **Client Secret**.  
     - Update the code with your credentials.

4. 🖼️ **Image Paths**  
   - The project references image files for playlists and UI components.  
   - Update the image paths in the code to match **your local system paths**. Example:  
     ```python
     playlist_image_1 = Image.open("D:/YourPath/images/playlist1.png")

