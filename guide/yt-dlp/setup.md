# Youtube video downloader setup

> [!NOTE]  
> This guide was last modified 2024-08-05.

## Windows

### Install FFmpeg with Winget

```bash
winget install ffmpeg
```

### Install yt-dlp with pip

```bash
pip install yt-dlp
```

### Usage

1. List all available options with: `yt-dlp -F <youtube url>`.
2. Check the `id` for the audio-only option with the highest `TBR` and the video-only option with the highest resolution and with the highest `TBR`. Use them for the next step.
3. Use the highest quality video and audio and then merge them and save it as an mp4: `yt-dlp -f <audio id>+<video id> --merge-output-format mp4 <youtube url>`.
