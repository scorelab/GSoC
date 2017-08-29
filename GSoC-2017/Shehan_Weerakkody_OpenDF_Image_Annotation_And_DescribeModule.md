# Project Name
OpenDF - Image annotation and describe module

## Student Info
Name : Shehan Weerakkody  
University : University of Colombo School of Computing  
E-Mail : shehanweer123@gmail.com  

### Project Abstract
Nowadays, digital forensic tools are often used to investigate cyber crimes, which are becoming more and more frequent. OpenDF is a tool for forensic analysis of disk data. By having an image description module that automatically recognises objects from the large amount of images that are available in a disk, it saves manual work for an investigator. Basically, there is a need to maintain all the objects detected in an image in a Database and make it searchable using keywords. Moreover, This project builds a REST API for image annotation.

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#6176600054824960)

### [GSoC Project Proposal](https://docs.google.com/document/d/1zIJYMrAOB18vv1cQM5rMUfw6zb4Tco50pu8Rn1nmvJA)

### [GitHub Organization Repo](https://github.com/scorelab/OpenDF)

### [GitHub Personal Repo](https://github.com/ShehanWeerakkody/OpenDF)

### [Commits during GSoC 2017](https://github.com/scorelab/OpenDF/commits/describe-image)

### [Project Demo Video](http://LinkToDemoVideo)

### [Project Wiki](https://github.com/ShehanWeerakkody/OpenDF/wiki/Image-Annotation-Module)

### [GSoC Blog](http://GSoCBlog)

### Work Summary
During the last three months in GSoC 2017 I have implemented an image annotation REST API for the OpenDF digital forensic tool. First of all I implemented a basic image recognition model using different pre-trained Convolutional Neural Network models such VGG16, VGG19 and RestNet50. With use of Flask python framework I implemented a REST API which takes image file UUID as the input and it returns the predictions as a JSON response.  

Then we use the Google Cloud Vision API to annotate the given image. This has a huge amount of performance improvement. The image annotation results will return within 3 seconds. Finally we Dockerized the application. Using this image annotation module users can predict the image content. Also, Investigation organizations can use following models based on their requirements by simply editting the properties.conf file.  

VGG16  
VGG19  
ResNet  
GoogleCloudAPI  

### What Covered
Implemented a base Image Recognition Model using pre trained models.  
Implemented a Flask bare bone skeleton for REST API.  
Developed the REST API to take a file UUID and send the predictions as a JSON response.  
Handle REST API Exceptions.  
Use Google Cloud Vision API for Image Annotation module.  
Dockerized the application.  

### What left
Need to implement an Elastisearch to get the actual file path for a given UUID.  

### Reference
https://keras.io/  
https://www.tensorflow.org/  
https://medium.com/@ageitgey/machine-learning-is-fun-part-3-deep-learning-and-convolutional-neural-networks-f40359318721  
http://www.image-net.org/challenges/LSVRC/  
https://ujjwalkarn.me/2016/08/11/intuitive-explanation-convnets/  
https://cloud.google.com/vision/docs/  
