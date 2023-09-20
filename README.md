# 🍽️ TensorFlow-Object-Detection

Welcome to the TensorFlow-Object-Detection project! This machine learning model detects food items in videos using TensorFlow and SSD MobileNet. The model is trained on the Common Objects in Context (COCO) dataset, which contains over 330,000 images spanning 80 object categories, including various food items.

The video input is initially processed by converting it into individual frames, and then the model calculates the accuracy of detection for each frame in the video. The results are displayed in a user-friendly format.

This project was conducted under the guidance of Prof. Mitali Mukherjee from the BSBE department at IIT Jodhpur. It was a subsection of the AR/VR app constructor for the digital food experience. 

## 👥 Contributors
- [@kashvi0](https://github.com/kashvi0)
- @Anurag-Kumar-Bharti

## 🍔 Digital Food Experiencing using AR/VR

**Team Members:**
- Arun Raghav S
- Anurag Kumar Bharti
- Kashvi Jain

## 🔍 Object Detection using TensorFlow

### TensorFlow
TensorFlow is a free and open-source software library for machine learning and artificial intelligence. It can be used across a range of tasks but focuses on training and inference of deep neural networks.

### 📚 Learning Curve
We followed the course on object detection on [YouTube](https://www.youtube.com/watch?v=yqkISICHH-U&t=2260s) and trained our own model to detect different hand gestures in images and real-time using a webcam.

We closely followed the steps provided by this [GitHub Repository](https://github.com/nicknochnack/TFODCourse). Our model was trained to recognize four hand gesture classes: Thumbs Up, Thumbs down, ThankYou, and Livelong. The model successfully detected these gestures in real-time.

📹 **Real-time Detection Video:** [link](https://drive.google.com/file/d/1qrBVgpO8663VbQpn2BKV_TSPXYzMnkoO/view?usp=sharing)

However, this model didn't perform well when trained for different food models as it identified objects incorrectly. So, we switched to using a pre-trained model on the COCO dataset.

### COCO-DATASET
COCO stands for Common Objects in Context, and it's a benchmark dataset for image recognition. It contains challenging, high-quality visual datasets for computer vision, primarily state-of-the-art neural networks. COCO is often used to benchmark algorithms for real-time object detection. It includes 80 object classes.

![COCO Dataset](images/Aspose.Words.a8591ec5-08ed-4132-b54c-d01279b4be20.004.png)

We experimented with three different models.

1) **First Model**
   - **LINK:** [custom-object-detection-using-tensorflow-from-scratch](https://towardsdatascience.com/custom-object-detection-using-tensorflow-from-scratch-e61da2e10087)
   - This model, using `ssd_mobilenet_v2_coco`, had low accuracy and inconsistent labeling.
   - We attempted to improve it by increasing the number of training steps and adding more images, but there were no significant changes in the output.

2) **Second Model**
   - **LINK:** [Real-time Object Detection using SSD MobileNet V2 on Video Streams](https://heartbeat.comet.ml/real-time-object-detection-using-ssd-mobilenet-v2-on-video-streams-3bfc1577399c)
   - We encountered an unresolved error that prevented us from using this model.

3) **Third Model**
   - **LINK:** [Object Detection using SSD Mobilenet and Tensorflow Object Detection API](https://medium.com/@techmayank2000/object-detection-using-ssd-mobilenetv2-using-tensorflow-api-can-detect-any-single-class-from-31a31bbd0691)
   - Out of all three models, the third one worked well and detected objects with high accuracy. So, we proceeded with it.

📷 **Object Detection Screenshots:**
![Food Detection](images/Aspose.Words.a8591ec5-08ed-4132-b54c-d01279b4be20.013.jpeg)

## 🎥 Object Detection in Video

We developed code to save frames from videos in JPG format and generate XML files for these frames. This approach allowed us to detect food items in videos effectively.

🖼️ **Screenshots:**

![Video Frames](images/Aspose.Words.a8591ec5-08ed-4132-b54c-d01279b4be20.015.jpeg)

🧰 **Code Screenshot:**

![Code](images/Aspose.Words.a8591ec5-08ed-4132-b54c-d01279b4be20.016.jpeg)

📝 **XML Generated:**

![XML](images/Aspose.Words.a8591ec5-08ed-4132-b54c-d01279b4be20.017.jpeg)

**Thank You**
