# PlaylistRipper
## Overview
PlaylistRipper is a Python-based personal music management tool that helps you access higher-quality audio for your Spotify playlists. It uses yt-dlp to download the best available audio formats from YouTube, enhancing your listening experience on Windows x64-based devices.

<img width="871" height="652" alt="Screenshot 2025-07-29 011712" src="https://github.com/user-attachments/assets/b62b5fd2-a677-4474-b422-02ab060d4d44" />

## Disclaimer
This software is intended for educational and personal use only. It allows users to explore and organize their Spotify playlists locally with improved bitrate and codec options.

⚠️ Important: Use responsibly. Downloading or sharing copyrighted content without proper authorization may violate copyright laws. The author does not support or encourage illegal use and is not responsible for any misuse or legal outcomes.

## License
[License](LICENSE.md)

## Requirements
Ngrok – Included with the project. You’ll need to create a free account and reserve a static domain for Spotify authentication.

Spotify Developer Account – Required to access playlist data. Create one for free [here](https://developer.spotify.com/dashboard) and follow the setup instructions to generate your credentials.

Portable Dependencies – No installation necessary. The following are included:

* Python

* FFmpeg

* Yt-dlp

* Spotipy

Thanks for checking out PlaylistRipper!
Feel free to report issues through my contact info or contribute to the project.

## Installation

1. Download the project in the releases tab of the GitHub repository

2. Extract the .zip

<img width="695" height="438" alt="Screenshot 2025-07-29 212938" src="https://github.com/user-attachments/assets/038debad-184a-4b86-af00-a851020f661e" />

3. Start *Winpython64-3.12.4.1.exe* in *PlaylistRipper/* and extract it into *PlaylistRipper\PlaylistRipper\Data\python*

<img width="2047" height="613" alt="Screenshot 2025-07-18 193610" src="https://github.com/user-attachments/assets/1ec6deeb-508e-4b2e-ae91-897fffbf1086" />

4. Create Ngrok account for free [here](https://dashboard.ngrok.com/signup) and [reserve a domain](https://ngrok.com/blog-post/free-static-domains-ngrok-users)

<img width="905" height="1073" alt="Screenshot 2025-07-18 193306" src="https://github.com/user-attachments/assets/d9ee4c37-2dac-454b-b4bd-34fe41a6f2b3" />

5. Create a Spotify Developers account for free [here](https://developer.spotify.com/dashboard) and create an app. Then put in your ngrok redirect domain name in as **Https://(your ngrok domain.app)/callback** and turn on web api and web playback sdk (may not be needed, but I already have them on and it worked for me)

6. open *PlaylistRipper\config.json* (open in Notepad, VS Code, or other) and input your Spotify client ID and client secret ID (both in the Spotify dev app), then put in the redirect URL **https://(your ngrok domain.app)/callback**, your authtoken [here](https://dashboard.ngrok.com/get-started/your-authtoken), and your ngrok domain [here](https://dashboard.ngrok.com/domains)

7. run the *Playlist_Ripper.exe*

8. It will take about a minute or so to open up the GUI. I have had various boot timings depending on internet speeds and the number of songs/playlists. It is verified on Windows 11 x64, Unknown as to reliability on other .exe supporting Operating Systems

Note: in total, will take up 5.68GB (6,103,691,093 bytes) as of 7/30/25

## Troubleshooting

1. If you get error codes **ERR_NGROK_3004 ngrok gateway error** or **ERR_NGROK_8012 failed to establish a connection**, wait ~10s and refresh, depending on internet speeds, the code may send out requests before ngrok is initialized, which causes the errors.

2. If it does not seem to be working, go into Task Manager and see if the .exe is running. If so, check the command prompt for errors or incompatibilities, and troubleshoot from there.

3. If the songs being downloaded are the music videos with sound effects or any unwanted music, run the *Playlist_Ripper5.exe*, which will download the top 5 results. The reason that is not the default download method is due to how inefficient it is to look through all the results when doing large playlists.
   
