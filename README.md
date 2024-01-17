# Interactive-Motion-Tracking-System-using-OpenCV-and-Python
## Introduction
The Python programming language, renowned for its open-source and library-rich nature, stands as a versatile platform with an ever-growing community of users. Its simplicity in syntax, error-finding ease, and swift debugging processes contribute to its user-friendly appeal, making it a favored choice in the rapidly expanding market.

This project, set within the expansive landscape of Python's capabilities, focuses on the intricate domain of motion detection and tracking. By harnessing the power of the OpenCV module, the ensuing guide embarks on a journey to provide a thorough exploration of techniques dedicated to identifying and tracking dynamic movements. Join us in unraveling the potential applications and insights this project has to offer in the realm of Python-based motion analysis.
## **Table of Contents**
1. **OverView**
2. **Getting Started**
   - Prerequisites
   - Important Libraries
     - Open CV
   - Installation
3. **Code Implementation**
4. **Summary**
5. **Results**
6. **Conclusion**
7. **References**
8. **Contributors**
## **1. OverView**
Leveraging Python for motion detection is facilitated by the myriad open-source libraries available within the Python programming language. The significance of motion detection extends to various practical applications, including its utility in online exam invigilation and enhancing security measures in establishments such as stores and banks. This project serves as a comprehensive guide to delve into the realm of motion detection, showcasing its versatility and applicability.
## **2.Getting Started**
### Prerequisites
No prerequisites are required to run this project.
### Important Libraries
Before we start the code implementation, let’s look at some of the modules or libraries we will use through our code for motion detection with a webcam. As we have discussed libraries play an important role in the fame of python. We are going to use Open CV for this project.
#### Open CV
OpenCV is an open-source library that can be used with many programming languages like C++, Python, etc. It is used to work on the images and videos and by using or integrating it with python’s panda/NumPy libraries we can make the best use of the OpenCV features.
### Installation
At first, you need to install the OpenCV-python module, to install the module just open your command prompt and type,
```
pip install OpenCV-python
```
## **3. Code Implementation**
1. To begin, install the OpenCV-python module by executing the following command in your command prompt:
   ```
   pip install OpenCV-python
   ```
   
2. Once the module is installed, proceed to import it into your Python script. Begin by reading the video using basic code.

3. Next, acquire two frames from the video or webcam to identify movement. Utilize the **cv2.absdiff()** function from the OpenCV module to find the difference between these frames, highlighting areas of movement.

4. Convert the resulting difference image to grayscale for clarity and subsequently apply Gaussian smoothing using **cv2.GaussianBlur()** to obtain a clear binary image.

5. Transform the smoothed image into a binary format by using the **cv2.threshold()** function in OpenCV.

6. Now, it's time to detect and track movements by following these steps:
   - Find contours in the binary image using **cv2.findContours()** in OpenCV.
   - Utilize the contours' details to outline them with different colors using **cv2.drawContours()** or draw rectangles around the contours. Achieve the latter by obtaining the contour's x, y position, width, and height with **cv2.boundingRect()**

7. In this implementation, we will draw rectangles around the detected contours.

Combine these steps to create a comprehensive Python script for motion detection and tracking.
## 4. **Summary**
This project focuses on implementing motion detection and tracking using the OpenCV-python module in the Python programming language. The initial step involves installing the necessary module through a simple command in the command prompt. Following installation, the script imports the OpenCV module and establishes the foundation for video processing by reading frames. Subsequently, the project employs the `cv2.absdiff()` function to identify differences between consecutive frames, utilizing grayscale and Gaussian smoothing for enhanced clarity. The resulting binary image is then processed to detect contours, marking regions of movement. The script concludes by outlining these contours with rectangles using the `cv2.boundingRect()` function. This comprehensive approach provides a practical guide to understanding and implementing motion detection and tracking for diverse applications, such as online exam invigilation or security surveillance in various settings.
## 5. **Results**
The results derived after the above code was run would be similar to what can be seen in repository.In the video, we can see that the man's motion in the Input video has been tracked. Thus, the output can be seen accordingly.However, in this code, the tracking would be done with the help of rectangular boxes around moving objects, similar to what can be seen in output video. 
## 6. **Conclusion**
- Python, known for its open-source nature and extensive libraries, offers diverse applications to users.
- In the context of motion analysis, the distinction between rest and motion is determined by an object's speed; a stationary object is at rest, while any degree of motion signifies its dynamic state.
- OpenCV, an open-source library compatible with multiple programming languages, becomes a potent asset when seamlessly integrated with Python's pandas/NumPy libraries, allowing for optimal utilization of OpenCV features.
- The core concept driving this project revolves around recognizing that a video is essentially a composition of static images known as frames. The detection process hinges on identifying differences between these frames, emphasizing the fundamental aspect of motion detection and tracking.
## 6. **References**
1. OpenAI Gym. (https://gym.openai.com/)
2. S Takemura, A Bharioke, Z Lu, A Nern, S Vitaladevuni… - Nature, 2013 - nature.com
3. CWG Clifford, MR Ibbotson - Progress in neurobiology, 2002 - Elsevier
4.  Vaishnavi Amira Yada,August 12, 2022,How to Perform Motion Detection Using Python.
## 7.**Contributors**
Nimeesha Vakacharla
