# Integrate ML module for LabelLab

## Student Info

* Name - Lakshyajeet Dwivedee	
* Email - lakshyajeet22@gmail.com
* GitHub Profile - https://github.com/laksh22
* Medium - https://medium.com/@laksh22
* Twitter - N/A

### Project Abstract
LabelLab allows the user to upload images and label them using bounding boxes and polygons. Currently, there is no way for the user to build models using the labelled dataset which they have created. The goal of the project is to create a pipeline which allows the users to train classification models using the images which have been uploaded and labelled on LabelLab.

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#6461961740484608)

### [GSoC Project Proposal](https://docs.google.com/document/d/1AYSI_DJW0vCTyZJDI2K1D52CqQx2I2tbN3qMI2FLfDc/edit?usp=sharing)

### [GitHub Organization Repo](https://github.com/scorelab/LabelLab)

### [GitHub Personal Repo](https://github.com/laksh22/LabelLab)

### [Commits during GSoC 2020](https://github.com/scorelab/LabelLab/commits?author=laksh22)

### [Project Demo Video](https://drive.google.com/file/d/1aDg-hLbYx82OHQ9Jo8Da4S6jmpAsLQ_0/view?usp=sharing)

### [GSoC Blog](https://medium.com/@laksh22/gsoc-2020-weekly-summaries-1ffd22617051)

### Work Summary
For GSoC 2020, I worked on adding a machine learning module to the LabelLab image annotation tool. This involved creating the client and server code for a dashboard which allows the user to create classification models. This dashboard also allows the user to train these models using the images which they have labelled using LabelLab. The user can then test the models and export them as well. For managing several models, a model management dashboard is also created through which the user can add, edit, or delete models.

### What Covered
1. Model management dashboard for adding, editing, deleting models
2. Sub-module for choosing labels to train on
3. Sub-module for choose image augmentation steps
4. Sub-module for training custom model
5. Sub-module for transfer learning
6. Sub-module for training an uploaded model
7. Sub-module for showing training accuracy and loss
8. Sub-module for testing a trained model
9. Sub-module for exporting a trained model in SavedModel, h5, and ONNX format

### What left
1. Adding tests

### Reference
1. [Tensorflow Keras API](https://www.tensorflow.org/api_docs/python/tf/keras)