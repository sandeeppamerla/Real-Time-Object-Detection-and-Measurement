# REAL-TIME OBJECT DETECTION AND MEASUREMENT 

In these days, measuring the dimensions of some objects using ruler or some measuring tools has become hectic. Finding the dimensions of an object has to be digitalized. In this project, we propose an algorithm where the dimensions of an object is measured in video streams. This project has a scope in many sectors such as Production sector where the size of the product has to be determined. Let us assume that a company is manufacturing the bricks and it wants to discard the bricks of inappropriate sizes then our system would help itin determining the uneven sized bricks for relinquishment. There are a lot of industrialbased applications where object dimensions measurement plays a vital role. We use standard python libraries such as OpenCV, NumPy etc.., to capture the photo and find the dimensions of the object. Some functions associated with the tuning of the images are used.

We are more interested in mechanisation and speedy working since the introduction of AI and IOT in the sphere of industrialization. The term "real time object detection and measurement" refers to getting the measurements of an object on screen while watching a picture in real time. Recognizing the object and its edges plays an important role in detecting the object. Edge detection is an important stage in image processing and handling, computer vision, and so on. There are several approaches for distinguishing an object and its edges. Edge Detection, the core topic in computer vision, is a method of handling a picture to determine the borders of an object. In this project, we are using one of the algorithms we developed to detect an item and estimate its size in a metric unit framework. We employed the thresholding approach for precise edge detection of the object. One of the primary benefits of this process is that it will lessen our workload and the difficulty of correctly measuring the thing. You just use a camera to determine the dimensions of an object in a couple of seconds. You only need to set your thing on white paper.

The implementation of this project is done using OpenCV library of Python. Theobject to be measured is placed on an A4 sheet. The A4 sheet can be aligned in any way. we will create a contours function that we allow us to first find the A4 paper and then to find the object inside it. So we will be using the same function to perform both of these tasks. we will apply some prepossessing to our coloured image. We will transform it into grayscale, then add some blur, then find the edges using the Canny edge detector and then apply some dilation and erosion. We use certain techniques to reduce the noise in the image and produce the correct form of image for the detection of the dimensions. Thus, the dimensions of the object is determined by following theabove suggested techniques.

# Methodology Flowchart

![fig1](https://user-images.githubusercontent.com/111385394/218642561-c63cf171-890b-4d17-b700-c5f8f022c1aa.JPG)
![fig2](https://user-images.githubusercontent.com/111385394/218642681-ca4d3fa4-8b84-440f-9748-6516c928416c.JPG)

# Procedure
1. Import cv2 and numpy library.
2. Computer Vision library is short termed as cv2 library which
helps totune the image as per our requirement and find the contours.
3. Numpy library is used to store the co-ordinates of the object in the image which helps to know the dimensions of the object.
4. Set the brightness to 160 whose id is 10.
5. Set the width to 1920 whose id is 3
6. Set the width to 1080 whose id is 4
7. You can either read the image from webcam or import the image from an external file.
8. We recommend you to import image from external file because
capturing an image from webcam produces the image of low resolution.
9. Resize the image if you feel that the existing image is too large.
10. We are aimed to detect the A4 paper in the picture.
11.Extract the image of paper and scale it and find the objects inside the paper
12. Find the Biggest Contour in the existing image by running a for loop.
13. Create a new python file utils.py where all the utilities are mentioned.
14. Define a function getContours()
➔Convert the image into Gray Scale
➔Convert the image into Gaussian Blur
➔ Use the Canny Edge detector to find the edges and define thethreshold.
➔User has the privilege to change the Threshold.
➔Define the kernel.
➔Apply Image Dilation to dilate the image.
➔Apply Image erosion to erode the image.
➔Display the image after you perform the above functions.
16. Define a function named findContours()
➔We can find the areas of contours and filter out based on minimum threshold.
➔Find the perimeter of the contour and find the corner points of the contour.
➔You have to make sure that the object is closed.
➔You can define a list and store the length of the suitable lengths.
17. Sort the final contours based on the size of the area.
18. Iterate over the list and find the contour of largest area.
19. Draw the contour of largest area.
20. Reorder the points so that the points must appear insorted order.
21. Warp the image.
22. Re-invoke the getContour function such that it detects the object in the paper.
23. After detecting the image, draw the lines over the selected co-ordinates and finally display the image.

# Advantages and Disadvantages
Advantages:
• It reduces man error and increases proficiency.
• It can be used easily.
• Less error is directly proportional to more profit.
• Not expensive that is it is low cost only a webcam is required.
Disadvantages:
• Saving output.The output given does not get backed up in any record hence there is a need for a backing system.

# Characteristics Of Project:
• It is a more convenient way to take measurements.
• Easy implementation
• Has a better future scope.
• It has accuracy.
• Fewer chances of human error.
• It will save money on instruments that we normally use to take measurements.
• It is easy to use and will save time and effort.

# Conclusion
As a result of this system, many improvements can be made to the industrial sector. The project successfully measures the dimensions of the object in real-time. Hence the computer vision (webcam device and code) is used to measure the dimensions in real-time. It captures the image from the realtime video frame and then displays its dimensions. A Canny edge detector is successfully used to detect the dimensions. This technique works fast and has many advantages and salient features that can be implemented in the real wo Hereby we conclude by claiming that our model is 98% accurate and can be used in industrial applications to discard the objects of inappropriate sizes.

# Future Scope
Machines are used in every part of human life. Machines work according to us but in today’s world, we work according to machines. The rush to soar high is immense. Hence, machines are important and so are the parts of them. If the parts do not fit well a machine cannot work properly. The dimensions of the objects sure make a great impact. This AI IOT based project will help in measuring the dimensions in real-time. It is convenient and easy to use. It also gives accuracy and trust in the product.

# Testing Data And Observation
![fig6](https://user-images.githubusercontent.com/111385394/218650233-61e81dc3-515a-4439-862d-35030c338488.JPG)
![fig5](https://user-images.githubusercontent.com/111385394/218650240-a4739e5e-2fc4-4276-93dd-86ce6cd92f97.JPG)
![fig3](https://user-images.githubusercontent.com/111385394/218650244-3a16b414-517d-4057-9479-86ddf4822c84.JPG)


