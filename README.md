

### File Structure:

- `README.md`: The ultimate guide to understanding and using the code.
- `extract_images.py`: Python script for extracting images from videos and editing their metadata.
- `requirements.txt`: List of required libraries and their versions.
- `videos/`: Directory for storing input video files.
- `images/`: Directory for storing output extracted images.

### Usage:

1. Clone the repository: `git clone https://github.com/your-username/extract-images-from-videos.git`
2. Install the required libraries: `pip install -r requirements.txt`
3. Place your video files in the `videos/` directory.
4. Run the script: `python extract_images.py`
5. Extracted images will be saved in the `images/` directory with updated metadata.

### Code Explanation:

The `extract_images.py` script contains the following steps:

1. Import the necessary libraries (cv2, datetime, piexif) for video processing and metadata editing.
2. Specify the paths for the input videos directory (`videos/`) and the output images directory (`images/`).
3. Iterate through each video file in the input directory.
4. Read the video file and get its frames per second (fps).
5. Initialize variables for frame extraction.
6. Extract frames at 5-second intervals and save them as images.
7. Get the video's datetime created and update the image's metadata with it.
8. Save the modified image with the updated metadata.
9. Release the video capture.
10. Print a message indicating the number of videos processed and images extracted.


This code allows you to extract images from multiple videos and edit their metadata using the piExifTool library.

## How it works:

1. Load the videos from the specified file path.
2. Read the video frames per second (fps).
3. Loop through each video and extract frames at 5-second intervals.
4. Get the metadata (datetime created) of the video.
5. Rename each extracted image with the video's datetime and frame number.
6. Update the image's EXIF metadata with the video's datetime.
7. Save the modified image with the updated metadata.
8. Release the video capture.

## Usage:

1. Specify the directory paths for the videos and the output images.
2. Run the code.
3. The extracted images will be saved in the specified output directory.
4. The images will have their metadata updated with the datetime information from the corresponding videos.

## Requirements:

- cv2 library: Install using `!pip install cv2`.
- piexif library: Install using `!pip install piexif`.

Please note that you need to have the specified libraries installed in order to run the code successfully.

Feel free to modify the code according to your specific requirements.

That's a brief overview of the code in the code.ipynb file. If you have any further questions, feel free to ask!
