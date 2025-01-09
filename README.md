# Bird Detection with YOLOv10

This project demonstrates how to use the YOLOv10 model to detect birds in videos using Google Colab. The repository includes steps for mounting Google Drive, preparing data, training a YOLOv10 model, and running inference on a video.


## Table of Contents
1. [Setup](#setup)
2. [Data Preparation](#data-preparation)
3. [Installing Packages](#installing-packages)
4. [Training the Model](#training-the-model)
5. [Inference on Video](#inference-on-video)
6. [Downloading Results](#downloading-results)

## Setup

1. **Mount Google Drive:**
   Ensure your dataset and configuration files are stored in Google Drive.

   ```python
   from google.colab import drive
   drive.mount('/content/gdrive')

  2. Prepare Data: Copy the dataset to the working directory and extract it.
    !scp '/content/gdrive/My Drive/bird_detection/data.zip' '/content/data.zip'
    !unzip '/content/data.zip' -d '/content/'
