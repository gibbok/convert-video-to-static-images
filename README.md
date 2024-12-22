# Convert Video to Static Images

This project allows you to extract static images (screenshots) from a video file at regular intervals.

## Features

- Supports input videos in `.mkv` and other common formats.
- Saves screenshots as sequentially numbered image files.
- Configurable screenshot intervals.

---

## How to Use

### Prerequisites

1. Ensure you have Python installed (version 3.8+ recommended).
2. Install [Poetry](https://python-poetry.org/) for dependency management.
3. Install FFmpeg, as it is required for processing video files. Follow the instructions for your operating system:
   - **Linux:** `sudo apt install ffmpeg`
   - **macOS (Homebrew):** `brew install ffmpeg`
   - **Windows:** Download from [ffmpeg.org](https://ffmpeg.org/download.html) and add it to your `PATH`.

### Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/gibbok/convert-video-to-static-images.git
   ```
2. Navigate to the project folder:
   ```bash
   cd convert-video-to-static-images/converter
   ``` 
3. Install dependencies:
   ```bash
   poetry install
   ``` 

### Usage

Run the script with the following arguments:

1. **Input video file:** Path to the video file (e.g., `/path/to/video.mkv`).
2. **Output folder:** Directory where screenshots will be saved (e.g., `/path/to/output/folder`).
3. **Interval (optional):** Time in seconds between screenshots (default is 5 seconds).
Example:

```bash
poetry run python extract_screenshots.py /path/to/video.mkv /path/to/output/folder --interval 5
```

The screenshots will be saved in the specified output folder as `.png` files, named sequentially.

# Convert Video to Video H265

This project allows you to compress a video in to H265.

Use as:

```bash
poetry run python compress_h265.py "/input.mkv" "/output"
```


### License

This project is licensed under the MIT License.
