# Fake Text Story Video Generator

This is a video creation tool that you can generate fake iMessage styled text story videos with text-to-speech, sound effects, and customizable backgrounds.
I'm pretty sure you came across those videos on tiktok and youtube shorts where two AI voice actors read out a fake text message conversation. This type of videos are fun and fairly engaging, but to make them either you need to pay for AI tools or edit videos yourself on tools like capcut, which costs money and very time consuming. That's why I created this website, to simply create fake text interface and render it into a video with voiceovers, background videos and sound effects. This tool will be helpful for those who looking for video automation tool for tiktok and youtube shorts. Try now and create your own viral shorts today.


Important: The preset video files I used cannot be uploaded on Github since they exceed the git LFS free limit of 1GB, so I'm attatching the video files here so that you can download them and try yourself. The video files should be saved under static - videos folder. 

Also, I tried deploying my python app on Render and Netlify, but their free tier have not enough memory for my app to process with the video rendering and capturing. I have uploaded another repo where you can use Google Cloud to upload your videos and use your credentials in the code to code to utilize cloud uploaded videos into video processing. I'm still working on the website deployment, so stay tuned. 

## Features

- Create realistic iMessage conversations
- Switch between sender and receiver messages
- Edit, delete, or add messages above or below
- Add sound effects to messages (Vine boom, notification, rizz)
- Choose from multiple voice actors using ElevenLabs API
- Select from various background video styles
- Customize profile image and name
- Download as MP4 video

## Requirements
(Refer to the contents below when you want to edit the script, I have already published the script on Web, using Render.)

- Python 3.8+
- FFmpeg (for video processing)
- Chrome/Chromium (for Selenium)
- ElevenLabs account with API key

## Setup

1. Install Python dependencies:
```bash
pip install -r requirements.txt
```

2. Run the Flask application:
```bash
python app.py
```

3. Open your browser and navigate to:
```
http://127.0.0.1:5001
```

## Usage

1. Enter your ElevenLabs API key and click "Fetch Voices"
2. Customize the chat interface:
   - Click profile image to upload a custom photo
   - Click the name to edit it
   - Select voice actors for sender and receiver
   - Choose your preferred background style

3. Create messages:
   - Type your message in the input field
   - Use the ⇄ button to toggle between sender/receiver
   - Press Enter or click Send to add message

4. Edit messages:
   - Click any message to:
     - Edit text
     - Switch sender/receiver
     - Add message above/below
     - Add sound effects
     - Delete message

5. Generate Video:
   - Click "Generate Video" button
   - Wait for processing
   - Video will download automatically

## Voice Requirements

Your ElevenLabs account needs access to these voices:
- Adam (male) - Some accounts with this voice doesn't provide the voice ID to the script, so the ID is hardcoded in the script.
- Natalie (female)
- Brian (male)
- Laura (female)

## Improvements
1. Website UI
2. Web deployment (still in progress)
