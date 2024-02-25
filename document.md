# Overview
In this project, I initially experimented with multiple pre-trained YOLO models from the Ultralytics library. However, the results were unsatisfactory. Subsequently, I implemented a custom tracker, but it did not yield significant improvements. To enhance accuracy, I analyzed the confidence scores of the detected bounding boxes to determine an optimal threshold for filtering out incorrect detections. Despite these efforts, due to time and resource constraints preventing training on dedicated 'person detection' datasets, I opted to utilize the rtdetr pre-trained model. After fine-tuning the bounding box threshold to 0.55, I achieved satisfactory results.

## Step 1
In this initial step, the objective is to detect individuals and draw bounding boxes around them.

## Step 2
Next, the task involves counting the number of detected individuals in the video.

## Step 3
Finally, we identify a specific area and tally the individuals present within it. For this purpose, I analyzed the center coordinates of each person's bounding box and determined if it fell within the specified area for counting.
