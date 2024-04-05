# Video Captioning Tool README

Welcome to the Video Captioning Tool, an automated solution designed to enhance videos with accurate and synchronized subtitles. This tool extracts audio from video files, transcribes the audio to text, and burns the resulting subtitles directly into the video, creating an accessible and enriched viewing experience.

## Features

- **Automatic Installation Checks**: Ensures necessary dependencies like `ffmpeg`, `Python3`, and `pip3` are installed.
- **Dependency Management**: Automatically installs required Python libraries.
- **Audio Extraction**: Utilizes `ffmpeg` to extract audio from the provided video file.
- **Speech-to-Text Transcription**: Leverages the `lightning-whisper-mlx` library for accurate audio transcription.
- **Subtitle File Creation**: Generates an SRT subtitle file from the transcription.
- **Subtitle Embedding**: Burns the generated subtitles into a new video file, preserving the original.

## Installation and Setup

### Prerequisites

- `ffmpeg`: Required for audio and video processing.
- `Homebrew` (for macOS users): Needed for installing `ffmpeg`.
- `Python3` and `pip3`: Necessary for running the transcription script and managing Python dependencies.

### Dependencies

- `lightning-whisper-mlx`: A Python package for audio transcription.

## How to Use

1. **Prepare Your Environment**: Ensure `ffmpeg`, `Python3`, and `pip3` are installed on your system. The script will attempt to install `ffmpeg` using Homebrew if it's not found.
   
2. **Install Python Dependencies**: The script will automatically install the `lightning-whisper-mlx` library.

3. **Run the Script**: With the script saved and executable, run it by passing the video file as an argument:
   ```bash
   chmod +x captionize
   ./captionize [video_path]
   ```
   Replace `[video_path]` with the path to your video file.

4. **Retrieve Your Captioned Video**: The script outputs a video file with embedded subtitles. The file is saved in the same directory as the original, with "_captioned.mov" appended to the original file name.

## Planned Improvements

- **Enhanced Language Support**: Extend transcription capabilities to support multiple languages.
- **Improved Subtitle Synchronization**: Refine subtitle timing to ensure even greater accuracy in text synchronization with spoken words.
- **Dynamic Subtitle Formatting**: Implement customization options for subtitle appearance, including font size, color, and positioning.
- **GUI Implementation**: Develop a user-friendly graphical interface to facilitate use by individuals unfamiliar with command-line operations.
- **Efficiency Optimizations**: Optimize script performance for handling large or multiple video files simultaneously.

## Support and Contribution

MIT Liocense. Do whatever you want with this.