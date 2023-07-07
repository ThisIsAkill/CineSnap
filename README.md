# Cinesnap
🎥 CineSnap: Lights, Camera, Frames! Capture the magic of your videos with this fun shell script. Extract frames at any interval to create stunning snapshots, funky GIFs, or movie previews. Simply specify the video file and frame frequency, sit back, and let CineSnap do the rest. Lights, camera, action! 📸🎞️

## Prerequisites

Before using CineSnap, ensure that you have the following installed on your system:

- [FFmpeg](https://ffmpeg.org/): A powerful multimedia framework for handling audio, video, and other media files.

## Usage

1. Clone the CineSnap repository to your local machine:
   ```bash
   git clone https://github.com/thisisakill/CineSnap.git
2. Navigate to the CineSnap directory:
   ```bash
   cd CineSnap
3. Make the shell script executable:
   ```bash
   chmod +x cinesnap
4. Run the script with the video file path and the desired extraction interval (in seconds) as arguments:
   <b>This example extracts frames every 10 seconds from the specified video file.</b>
   ```bash
   ./cinesnap path/to/video.mp4 10
5. The extracted frames will be saved in a directory named after the video file (without the extension) within the CineSnap repository.

## Contributing
Contributions to CineSnap are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License
CineSnap is open source and available under the **MIT License**.
