# EyeGazeTrackingCorners
An open dataset with 1600 labeled images from eye gaze tracker videos collected on the da Vinci Standard Surgical System. Images are labeled with 4 eye corner bounding boxes and 2 eye bounding boxes.

# Dataset Description
This is a hand-labeled dataset on images taken with an eye gaze tracker retrofitted for the da Vinci Standard Surgical System. Images are from 44 participants and the frames were extracted at random from the eye gaze videos. The images are scaled to 640x640 from 1280x480 sized images and can be scaed back using the opencv cv2.resize with the 'linear' option. The images are of both eyes and there are 6 labels with bounding boxes around all four eye corners and around the two eyes.

# Dataset Structure
The 1600 images were split into 80% for training, 10% for testing, and 10% for validating for your convenience. The dataset follows the conventional YOLO format with each image having a corresponding label file with the same file name but with the '.txt' extension. There are separate image/label files for each of train/test/ and valid as seen below:
1. train
   * images
   * labels
2. test
   * images
   * labels
3. valid
   * images
   * labels

# Label format
The labels are formatted such that: [class ID, x-center, y-center, width, height]. And the class names are as follows:
- 0: Right Eye Inner
- 1: Right Eye Outer
- 2: Left Eye Outer
- 3: Left Eye Inner
- 4: Right Eye
- 5: Left Eye
# File Download
Just download the 'EyeImageDataset.zip' file and you should be good to go.

