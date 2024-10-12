# OpenPose: Pose Detection Using OpenPose

This project implements pose detection using the OpenPose framework. The application processes a video from YouTube, cuts a specific segment, and performs pose detection to visualize the results.

## Features
- **Pose Detection:** Utilizes OpenPose to detect human poses in a video.
- **Video Processing:** Downloads a YouTube video, cuts a specific segment, and processes it for pose detection.
- **Output Visualization:** Generates output video with detected poses visualized.

## Prerequisites
- Python 3.x
- The following Python libraries must be installed:
  - `numpy`
  - `ffmpeg-python`
  - `yt-dlp`

You can install the required libraries using pip:
```bash
pip install numpy ffmpeg-python yt-dlp
```
## Project Structure
```bash
.
├── openpose/                # Cloned OpenPose repository containing the model and scripts
│   ├── build/               # Build directory for OpenPose
│   ├── models/              # Directory containing OpenPose models
│   ├── scripts/             # Scripts for installing dependencies
│   └── ...                  # Other OpenPose files and dependencies
├── LSE_OpenPose.ipynb      # Main Jupyter Notebook for pose detection
└── README.md                # Project README file
```
## How It Works

-**Clone OpenPose Repository**: The OpenPose repository is cloned from GitHub, which contains the necessary scripts for pose detection.
-**Install Dependencies**: Required system and Python dependencies are installed.
-**Build OpenPose**: The OpenPose library is built using CMake.
-**Download Models**: OpenPose models for pose detection are downloaded.
-**Video Processing**:
The specified YouTube video is downloaded.
A segment (from 15 to 20 seconds) is cut from the video.
-**Pose Detection**: OpenPose processes the cut video segment to detect poses and generates an output video.

## Running the Project
Open the Jupyter Notebook:
`jupyter notebook LSE_OpenPose.ipynb`

Follow the instructions in the notebook to clone the OpenPose repository and install dependencies.

Set the YOUTUBE_ID variable to the desired YouTube video ID.

Run the notebook cells to download the video, cut the desired segment, and perform pose detection.

## Example Output
After running the pose detection, an output video (output.mp4) will be generated, showcasing the detected poses from the specified video segment.

## Contributing
Contributions, issues, and feature requests are welcome! Feel free to check the issues page for new ideas.

## License
This project is licensed under the MIT License.

## Acknowledgments
OpenPose for pose detection functionalities.
YouTube-DL and FFmpeg for video processing.
Google Colab for providing a cloud-based Jupyter notebook environment.
