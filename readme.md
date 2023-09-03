# Object detection project

Task is to detect objects - icy bridges, on images coming from road cameras.

- Data from ["rtp-aws"](https://github.com/rtp-aws/devpost_aws_disaster_response/tree/main/icy-bridge), I also tried to solve this problem.
- Made annotattion with ["CVAT.ai"](https://www.cvat.ai/) with free account
  - Created 2 classes:
    - bridges
    - icy_bridges
- Split data into train and validate batches
- Trained Yolo v8 image detection model
- Validated the trained model

Its a simple solution to try solve the problem and learn the CV technologies and object detection. 

Here is what it was able to detect:
!["How it should be"](/runs/detect/val2/val_batch0_labels.jpg)
!["What model detected"](/runs/detect/val2/val_batch0_pred.jpg)
!["Confusion Martix"](/runs/detect/val2/confusion_matrix_normalized.jpg)

## useful resources:
Train Yolov8 object detection on a custom dataset [https://www.youtube.com/watch?v=m9fH9OWn8YM](https://www.youtube.com/watch?v=m9fH9OWn8YM)