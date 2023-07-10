<h1 align="center">CineSnap 🎥</h1>
🎥 CineSnap: Lights, Camera, Frames! Capture the magic of your videos with this fun shell script. Extract frames at any interval to create stunning snapshots, funky GIFs, or movie previews. Simply specify the video file and frame frequency, sit back, and let CineSnap do the rest. Lights, camera, action! 📸🎞️
<br></br>

## Features

- **Frame Extraction**: Extract frames from a video file at specified intervals.
- **Time Interval Extraction**: Extract frames at regular time intervals, e.g., every 10 seconds.
- **Custom Timestamp Extraction**: Extract frames at specific timestamps provided in a file.
- **Pause Before Capture**: Introduce a pause before capturing each frame to improve image quality.
- **Timestamps and Duration**: Generate a text file with frame numbers, video timestamps (in frames), and video durations (in hh:mm:ss format) for each extracted frame

## Prerequisites

Before using CineSnap, ensure that you have the following installed on your system:

- [FFmpeg](https://ffmpeg.org/): A powerful multimedia framework for handling audio, video, and other media files.

## Commands

- **'<video_file>'**: Path to the video file from which frames will be extracted.
- **'-ts <interval>'**: Extract frames at the specified time interval (in seconds). For example, '-ts 10' will extract frames every 10 seconds.
- **'-tsfile <timestamps_file>'**: Extract frames at the timestamps provided in the specified file. The file should contain one timestamp per line, in seconds.

## Usage

1. Clone the CineSnap repository to your local machine:
   ```bash
   git clone https://github.com/thisisakill/CineSnap.git
   ```
2. Navigate to the CineSnap directory:
   ```bash
   cd CineSnap
   ```
3. Make the shell script executable:
   ```bash
   chmod +x cinesnap
   ```
4. Run the script with the video file path and the desired extraction interval (in seconds) as arguments:
   ```bash
   ./cinesnap <video_file> [-ts <interval> | -tsfile <timestamps_file>]
   ```
5. The extracted frames will be saved in a directory named after the video file (without the extension) within the CineSnap repository.

## Examples

```bash
#Extract frames every 10 seconds from video.mp4
./cinesnap video.mp4 -ts 10
```

```bash
#Extract frames at the timestamps specified in timestamps.txt
./cinesnap video.mp4 -tsfile timestamps.txt
```
## Output

- Extracted Frames: The frames extracted from the video will be saved as individual images in the same directory as the video file. The images will be named in the format "frame_1.jpg", "frame_2.jpg", and so on.
- Timestamps File: When using the **'-ts'** or **'-tsfile'** options, CineSnap generates a text file named "extracted_frames_timestamps.txt" in the same directory as the video file. This file contains the frame number, video timestamp (in frames), and video duration (in hh:mm:ss format) for each extracted frame.

## Contributing
Contributions to CineSnap are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License
CineSnap is open source and available under the **GPL-3.0 License**.
