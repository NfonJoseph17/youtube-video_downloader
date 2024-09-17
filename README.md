# youtube-video_downloader
This Python script allows you to download YouTube videos in the highest available resolution using the pytube library. The program provides a graphical interface to select the save directory using tkinter’s file dialog.

Features

	•	Download YouTube videos in the highest available resolution (MP4 format).
	•	Use a graphical file dialog to select the download location.
	•	Handles SSL certificate issues by using certifi for SSL verification.

Requirements

	•	Python 3.x
	•	pytube library
	•	certifi library
	•	tkinter (for GUI file dialog)

Setup Instructions

1. Install Required Python Libraries

Before running the script, you need to install the required libraries. You can do this using pip:
pip install pytube
pip install certifi

2. Running the Script

Once the required libraries are installed, you can run the script directly. The script will ask you for the YouTube video URL and allow you to choose a directory to save the downloaded video.

3. Example Usage
   python youtube_downloader.py

1.	Enter the YouTube video URL when prompted.
	2.	Choose a save location through the graphical folder dialog.
	3.	The video will download to the selected folder.

4. Handling SSL Errors

In case of SSL certificate issues, the script uses the certifi package to bypass the problem. The following line ensures SSL verification works correctly:
ssl._create_default_https_context = ssl._create_unverified_context
