# Rewrite ImageLab backend

## Student Info

- Name - Kaveesha Dinamidu
- Email - [kaveesha.19@cse.mrt.ac.lk](kaveesha.19@cse.mrt.ac.lk)
- GitHub Profile - [kaveeshadinamidu](https://github.com/kaveeshadinamidu)
- Medium - [@kaveesha.19](https://medium.com/@kaveesha.19)

# Project Abstract

ImageLab is a standalone tool which supports anyone to get started with image processing related concepts and techniques in an interactive, less logical way. ImageLab electron project is a
cross-platform application containing image processing functions that are associated with
OpenCV. This application enables any user to test and implement image processing functions and
get an idea about image processing.

## [GSoC Project Page](https://summerofcode.withgoogle.com/programs/2022/projects/9njzCFJk)

## [GSoC Project Proposal](https://drive.google.com/file/d/1rdi8WWZB8QI322vNQpXUZQx8dZ-ItCbh/view?usp=sharing)

## [GitHub Organization Repo](https://github.com/scorelab/imagelab)

## [GitHub Personal Repo](https://github.com/kaveeshadinamidu/imagelab)

## [Commits during GSoC 2022](https://github.com/scorelab/imagelab/commits?author=kaveeshadinamidu)

## [Project Demo Video](https://drive.google.com/file/d/1vN04vmGKFcaNro7UmoDF8c5tJ19boRpR/view?usp=sharing)

# Work Summary

Integrated the image proccessing functions in the UI with the backend functions. Here opencvjs is used to implement the image processing functions. All the functions and the controllers are implemented in the most prominent way using classes and objects. As well as functionality added to the user interface elements (execute, reset, delete).

- Discussed about the approach to implement the image processing functions.
- Implement the functions for the image processing and integrated them with the user interface.
- Test the implemented functions and fix the raised bugs.
- Discussed about the issues faced during the development with the mentors.
- Demonstrating the work done and attending meetings with the mentors.
- Test the whole project and fix the raised bugs.

# What Covered

- Implement the functionality of the user interface elements.
  - Execute, Reset and Delete functionality in the workspace.
- Implemented the image proccessing functions
  - Basic operations
    - Read Image
    - Write Image
  - Geometric operations
    - Rotate Image and Resize
    - Affine Image
    - Scale image
  - Drawing operations
    - Draw line
    - Draw ellipse
    - Draw circle
    - Draw rectangle
    - Draw text
  - Blurring operations
    - Apply blur
    - Gaussian blur
    - Median Blur
  - Filtering operations
    - Bilateral Filter
    - Pyramid up
    - Box filter
    - Pyramid down
    - Erosion
    - Dilation
    - Morphological filter
- Integrated the operator details interface with the functions.
- Added the validations related with the operators and their flow.
- Operation execution mechanism added.
- Operation binding mechanism added according to the block order.
- Code refactored and commented.
- Documentation updated.

# What left

- Implement the other image proccessing functions.
- Implement the functions related with the workspace (Undo/Redo).
- Implement the workspace save,open functions.

# References

- [OpenCV.js](https://docs.opencv.org/3.4/d0/d84/tutorial_js_usage.html)
- [Electron Js](https://www.electronjs.org)
- [OOP in JS](https://www.geeksforgeeks.org/introduction-object-oriented-programming-javascript/)
- [OpenCV in Java](https://docs.opencv.org/4.x/d9/d52/tutorial_java_dev_intro.html)
