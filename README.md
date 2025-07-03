#  🚘 Vehicle License Plate Detection using YOLOv8 and OCR

## Project overview
This project combines YOLOv8 (You Only Look Once version 8) and OCR (Optical Character Recognition) to detect vehicle license plates in images and convert them into readable text data.
The pipeline works in two stages:
1. Object Detection with YOLOv8:
   YOLOv8 is used as a real-time object detection model to locate license plates in an image or video frame. Once detected, the model provides bounding box coordinates for each license plate.
3. Text Extraction with OCR:
   After detecting the license plate, OCR is applied to the cropped region to extract the characters and transform them into machine-readable text.

## Results and Performance

### YOLOv8 Detection Performance
- The accuracy curve indicates that the model successfully learned during the training process.
<img src="https://github.com/user-attachments/assets/4322fd92-bc49-4f03-9098-7e8f50b901c3" width="400">
- I used YOLOv8 Nano, which showed good confidence in detecting license plates from images.
![image](https://github.com/user-attachments/assets/a883289f-ee6d-4ec4-a02f-5cc548f3733d)

### OCR Text Detection Performance

![image](https://github.com/user-attachments/assets/6510c382-4326-4615-a792-23b5cba8b65f)

OCR still has some limitations. The average confidence score for text detection was around `45%`, meaning many detections were either inaccurate or failed.
In several cases, the license plate was clearly visible to humans but was either poorly recognized or not detected at all by the OCR engine.

## Conclusion
This project demonstrates the potential of combining YOLOv8 for object detection and OCR for text extraction to automate license plate reading. 
While object detection performed well, OCR still requires improvement to handle real-world variability in image quality and plate design.
With further optimization, this system can be developed into a reliable smart traffic monitoring or automated vehicle entry solution.

## Technologies used
`YOLO` `OCR` 
