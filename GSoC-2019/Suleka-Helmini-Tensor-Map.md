# Project Name

TensorMap

## Student Info

- Name: Suleka Helmini
- Email: sulekahelmini96comp@gmail.com
- University: Informatics Institute of Technology
- GitHub Profile: https://github.com/suleka96
- LinkedIn Profile: https://www.linkedin.com/in/suleka-helmini-09803b132/

### Project Abstract

TensorMap is a web application that will allow users to create machine learning algorithms visually. TensorMap supports reverse engineering of the visual layout to a TensorFlow implementation in Python. The goal of the project is to let beginners play with machine learning algorithms in TensorFlow with less background knowledge about the library. 

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/?fbclid=IwAR25OLx_wNZgAi9Sleg4VJl502SEfXnWbFg7WEnOpm9Ddy6y7--rYVFPiCc#4742286959706112)

### [GSoC Project Proposal](https://docs.google.com/document/d/1KCu9tV7zQ-qWWUerVCmbilxquJGnyTQrCV8mu9tZ9Hg/edit?usp=sharing)

### [GitHub Organization Repo](https://github.com/scorelab/TensorMap)

Note: We worked directly on the organization repo using branches to manage our work. Thus, there was no need to create a fork. Beacause of this reason I did not include GitHub Personal Repo link.

### [Project Wiki](https://github.com/scorelab/TensorMap/wiki)

### [Commits during GSoC 2018](https://github.com/scorelab/TensorMap/commits?author=suleka96)

### Pull Request links

* [PR 1](https://github.com/scorelab/TensorMap/pull/8)
* [PR 2](https://github.com/scorelab/TensorMap/pull/24)
* [PR 3](https://github.com/scorelab/TensorMap/pull/28)
* [PR 4](https://github.com/scorelab/TensorMap/pull/34)
* [PR 5](https://github.com/scorelab/TensorMap/pull/35)


### Work Summary

For GSoC 2019, 3 students were chosen to work on TensorMap. I mainly worked on developing the Flask backend for TensorMap and I also worked on adding logic and UI to several frontend components.

### What was Covered

Backend 
 * Setup initial backend architecture
 * Implemented backend routes to handle auto-generating of python Tensorflow (Keras) code according to the created drag-and-drop model to:
   * Initialize environment for code auto-generation according to the experiment type (Binary Classification, Multiclass Classification, Regression)
   * Add new Keras layer
   * Edit layer
   * Delete layer
   * Specify experiments configurations (number of epoch, loss function, etc)
   * Specify pre-processing information (features, labels, train and test splits, etc)
   * Download auto-generated code file
   * Write validation for experiment type and model-specific information
   * Remove initialized environment information
 * Implement database structure for application
 * Implement backend routes to handle pre-processing of data:
   * Upload CSV data
   * Render CSV data
   * Perform CSV manipulations:
     * Add data row
     * Edit data row
     * Delete data row
     * Delete column
   * Specify features, labels and train percentage for the experiment
   * Download edited CSV
 * Implement backend route to execute created model:
   * Create Keras compatible JSON to generate Keras model from received layer information
   * Provide progress of training for each epoch
   * Provide resultant metric values according to experiment type 
 
 Frontend
  * Implement logic and user interface for uploading data CSV
  * Implementing logic and user interface for visualizing the uploaded data and let users perform manipulations on data:
     * Add data row
     * Edit data row
     * Delete data row
     * Delete column
     * Sort column
     * Filter column
     * Search for data in table 
 

### What is left

* Testing
* Improving Documentation

### Project Demo

As mentioned before, I mainly worked on the backend of the application thus, I have only included some screenshots of the frontend components I implemented. 

* Add data view
![image](https://drive.google.com/uc?export=view&id=1LJwdkErBmrJeJaU7-PL9YRV6jdA_uPeH)

* Visualize data view
![image](https://drive.google.com/uc?export=view&id=1WqBjYzMS6WgiQD0lMC1AG_mS7DzeO9Dw)

### Reference

* [Tensorflow Keras](https://www.tensorflow.org/guide/keras)
* [React JS](https://reactjs.org)
* [Flask](https://flask.palletsprojects.com/en/1.1.x/)
* [material-table](https://material-table.com/#/)
* [SQLAlchemy](https://www.sqlalchemy.org)
