# ImageLab - extend the functionality

## Student Info

* Name - Sahan Dissanayaka
* Email - [tsahandisaai@gmail.com](tsahandisaai@gmail.com)
* GitHub Profile - [SahanDisa](https://github.com/SahanDisa)
* Medium - [@tsahandisaai](https://tsahandisaai.medium.com/)
* Twitter - [@TSahan998](https://twitter.com/TSahan998)

### Project Abstract
ImageLab is a standalone tool which supports anyone to get started with image processing related concepts and techniques in an interactive, less logical way. So, this tool enables and also motivates the fresh users to understand how image processing concepts work by interacting with ImageLab. Moreover, for the users who are already comfortable with image processing tasks ImageLab offers a test environment before they move ahead with actual implementation or development.

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#6076916190150656)

### [GSoC Project Proposal](https://docs.google.com/document/d/1QXV-v3lxWuXMCQp3k9prJTfm6odjIrdc9pqNsxuKfCY/edit#heading=h.3t1vo9whdrr2)

### [GitHub Organization Repo](https://github.com/scorelab/ImageLab)

### [GitHub Personal Repo](https://github.com/SahanDisa/imageLab)

### [Commits during GSoC 2021](https://github.com/scorelab/ImageLab/commits?author=SahanDisa)

### [Project Demo Video](https://drive.google.com/file/d/1SVIchmc2v9ikVRZJau7H3iNfLFyrdEeb/view?usp=sharing)

### [GSoC Blog](https://tsahandisaai.medium.com/)

### Work Summary

Extends the current functionalities to the next stage with the core objective of gaining the most prominent concepts in the image processing domain with the help of the OpenCV library. Also, provide fundamental image processing exercises via predefined operator streams/pipelines.
Provide better usability and user experience with the provided operators and able to provide a fully functional image processing tool for the end-user. Improved the current architecture to next step in order to perform easy and robust way of adding new OpenCV operators to the ImageLab dashboard.

- Discussed the improvements can be applied to the ImageLab architecture and refine it.
- Improve the current functionality to the next stage with prominent features.
- Finalize the further developed mockups and implement a complete user interface with newly proposed functionality.
- Fixing and solving issues and blockers occurred during the implementation phase with the support and guidance of mentors.
- Demonstrating the work and attending meetings with the mentors.
- Update and deliver the improved version of project documentation as a wiki.
- Testing the developed features and add test cases and reporting bugs fixes.

### What Covered
- Improvements applied to the ImageLab architecture.
    - Packaging the controllers according to relevant image processing operation section
- Improve the current functionality to the next stage.
    - Extended geometric transformation operators.
        - Affine Transformation (cv:: wrapAffine, cv::getRotationMatrix2D)
        - Image Scaling (cv::resize)
        - Color Maps (cv::applyColorMap)
    - Extended filtering operators.
        - Bilateral Filter (cv::bilateralFilter)
        - SQRBox Filter (cv::sqrBoxFilter)
        - Filter2D (cv::filter2D)
        - Pyramids Operations
    - Morpholigical operators.
    - Drawing operators.
        - DrawLine
        - DrawArrowedLine
        - DrawRectangle
        - DrawEllipse
        - AddText
    - Transformation operators.
        - Laplacian Transformation (cv::Laplacian)
        - Distance Transformation  (cv::distanceTransform)
    - Sobel derivation for the edge detection.
        - Sobel Operator (cv::Sobel)
        - Scharr Operator (cv::Scharr)
    - Contour operators for draw and find contours in images.
        - Find contours(cv::findContours,cv::drawContours)
        - Convex Hull (cv::convexHull)
        - Image Moments (cv::moments, cv::contourArea, cv::arcLength)
    - Miscellaneous operations for edge detection.
        - Canny Edge Detection (cv::Canny)
        - Hough Line Transform (cv::HoughLine)
    - Histogram operations for image analysing.
        - Histogram Equalization (cv::equalizeHist)
        - Histogram Calculation (cv::calcHist, cv::normalize)
        - Template Matching (cv::matchTemplate, cv::minMaxLoc)
- Improve the current properties pane with rich interactive components like sliders.
- Visulization through the histograms for the both RGB and Gray Images.
- Validation mechanism to validate openCV operation order.
- Operator execution mechanism.
- Code commenting.
- Junit Testing for the major operators.
- Improved [Documentation](https://sahandisa.github.io/imagelab/) as a jekyll website and include applications as a wiki.  

### What left
- Improve the operator pipeline to remove a certain operator from the stream.
- Watershed algorithm for isolate objects in the image.
- Exporting openCV operation order as an illustration of the pipeline.

### Reference
- [OpenCV docs - v3.0](https://docs.opencv.org/java/3.0.0/)
- [OpenCV docs - v3.4.9](https://docs.opencv.org/3.4.9/javadoc/index.html)
- [Java 1.8 docs - v3.4.9](https://docs.oracle.com/javase/8/docs/)
- [Java design patterns](https://www.journaldev.com/1827/java-design-patterns-example-tutorial)
- [JavaFX 1.8 docs - v3.4.9](https://docs.oracle.com/javase/8/javafx/api/toc.htm)
- [Getting started with JavaFX 8](https://docs.oracle.com/javase/8/javafx/JFXST.pdf)
- [Maven repo](https://mvnrepository.com)
- [Jekyll docs](https://jekyllrb.com/docs/)
- [Ruby docs](https://ruby-doc.org)
- [MIT Scratch](https://scratch.mit.edu/projects/editor/?tutorial=getStarted)