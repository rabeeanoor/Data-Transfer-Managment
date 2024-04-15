
# Camera Monitoring Data Management Script

## Description:
This script is used to manage video and image data from multiple cameras based on specific criteria. For each company and its associated cameras, the script will:

1. Check the main folder for the latest five date folders.
2. Copy videos and images from these date folders to a saving folder.
3. Delete any older date folders in the saving folder, keeping only the latest five.

## Prerequisites:

- Python 3.x
- The following Python libraries: os, shutil, datetime

## Usage:

1. Ensure that the `fix_data` dictionary at the beginning of the script is correctly populated with company names and their associated cameras.
2. Modify the `main_folder` variable to point to the directory where the camera data is stored.
3. Modify the `saving_folder` variable to point to the directory where you want the latest data to be saved.
4. Run the script.

## Functionality:

- `update_video_data_no_camera(main_folder, saving_folder)`: This is the primary function that performs the data management tasks. It takes in two arguments:
  - `main_folder`: The directory where the camera data is stored.
  - `saving_folder`: The directory where the latest data will be saved.

## Note:

- Ensure you have adequate permissions to read from `main_folder` and write to `saving_folder`.
- Always backup your data before running scripts that modify or delete files.
