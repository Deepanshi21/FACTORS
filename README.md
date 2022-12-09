# **FACTORS: Fine-grained Apparel category Classification & Try-On Recommender System**

## **PROJECT OVERVIEW:** 
Pandemic has played a vital role in how the people in the world operate. Where everything was offline, including education, meeting with people, etc., this sudden change in the world being shut completely, everything was forced to shift from the conventional to unconventional means. 

With this project, we aim to break this barrier between customers and brands to aid customers in trying on the clothes at their own convenience. Our project helps us to eliminate the shortcomings in the already established world of online shopping where the customers get the luxury to see how the clothes sit on their bodies, in the comfort of their homes.

The project we proposed is based on the VITON dataset, which consists of over 16,000 image pairs of clothing items along with the images of the person wearing them. Our project can be included in existing clothing website brands to cater to the users to virtually try on the clothing at their own comfort. The project can be further extended into suggesting clothes based on their body shapes and sizing where we'd be able to give similar suggestions based on their clothing choices and suggestions of clothing which would be flattering on their bodies.

## **PROJECT OUTCOMES:** 
The project is designed by the help of deep learning with the implementation of an interactive module where people can input their image and in turn find their desired clothing on their bodies. The project is divided into several modules: 

1. Human Segmentation: The image inputted by the user will contain all the background and disturbances, which must be eliminated or segmented for further processing. This method of human segmentation must be done by U2 net. The human body is separated from the background and retrieved for further processing. 

2. Predicting the posing of the human: The COCO format is used to convert the image format dataset to a specific JSON structure. Each body part is given a number with point pairs. The key points are generated for the pose which is used in the further parts of the code. 

3. Human Parsing: Human parsing is the task of segmenting a human image into different fine-grained semantic parts such as head, torso, arms and legs. The clothing and the body parts in the user’s image are then parsed to find the definitive part where the clothing lies and where the body part is exposed. 

4. Clothing warping: The clothing is warped and transformed according to the points of the human body to be superimposed on it. 

## **TECHNOLOGIES USED:** 
VITON dataset contains 16253 image pairs composed of an upper-body garment. Images are divided into training and test sets with 14, 221, and 2, 032 image pairs, respectively.

LIP (Look Into Person) human parsing is done for human segmentation. The LIP dataset is a large-scale dataset focusing on semantic understanding of a person. It contains 50,000 images with elaborated pixel-wise annotations of 19 semantic human part labels and 2D human poses with 16 key points. The images are collected from real-world scenarios and the subjects appear with challenging poses and view, heavy occlusions, various appearances and low resolution.

U2 net is used for the deep learning model in our project. U2-Net is a two-level nested U-structure architecture that is designed for salient object detection (SOD). This architecture allows the network to go deeper, attain high resolution, without significantly increasing the memory and computation cost.U2 net is used to train on our data since it has a two-level nested U-structure architecture that is designed for salient object detection (SOD)

Image uploaded by the user is tested on the trained model where parsing and segmentation are done, and the clothing is warped on the person's body.

**The software tools used by this system are:**
1.	Python 
2.	OpenCV [Open-Source Python library for CV]
3.	PyTorch
4.	U2 Net 
5.	Tensor Flow
6.	Scikit image

## **ARCHITECTURE OF THE PROJECT:**

![unnamed](https://user-images.githubusercontent.com/79203522/206647528-7bcb3f98-b383-4766-8c18-b48424db5273.png)

## **PROJECT SCREENSHOTS:**

![unnamed (3)](https://user-images.githubusercontent.com/79203522/206646317-08160da2-ed04-4a87-98bd-33e02275e16f.png)

![unnamed (7)](https://user-images.githubusercontent.com/79203522/206646691-b3478c12-0722-4c14-91d9-225dc4ebe3c1.png)

![unnamed (8)](https://user-images.githubusercontent.com/79203522/206646722-b9d6faed-8d69-4b55-ad6a-5382cc974e06.png)

![unnamed (9)](https://user-images.githubusercontent.com/79203522/206646736-db6b214c-4e0c-46a2-ab95-de5a9a379c9d.png)
 
Tested this system by uploading the photo:

![unnamed (1)](https://user-images.githubusercontent.com/79203522/206646778-94215101-9b66-469a-9f1f-e3b6decd944c.png)

Final photo outcome:

![unnamed (10)](https://user-images.githubusercontent.com/79203522/206650661-0f30d924-e8f8-4b85-a26a-1059c08c22e0.png)

**You can find the working video of the project here:**

https://youtube.com/playlist?list=PL7DJv6PVIMUdePq4FMyJfWkr1UqeuRSmC
