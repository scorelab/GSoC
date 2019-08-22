# Project Name

TensorMap

## Student Info

- Name: Suleka Helmini
- Email: sulekahelmini96comp@gmail.com
- University: Informatics Institute of Technology
- GitHub Profile: https://github.com/suleka96
- LinkedIn Profile: https://www.linkedin.com/in/suleka-helmini-09803b132/

### Project Abstract

TensorMap is a web application that will allow the users to create machine learning algorithms visually. TensorMap supports reverse engineering of the visual layout to a Tensorflow implementation in Python. The goal of the project is to let beginners play with machine learning algorithms in Tensorflow without less background knowledge about the library. 

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/?fbclid=IwAR25OLx_wNZgAi9Sleg4VJl502SEfXnWbFg7WEnOpm9Ddy6y7--rYVFPiCc#4742286959706112)

### [GSoC Project Proposal](https://docs.google.com/document/d/1KCu9tV7zQ-qWWUerVCmbilxquJGnyTQrCV8mu9tZ9Hg/edit?usp=sharing)

### [GitHub Organization Repo](https://github.com/scorelab)

### [GitHub Personal Repo](https://github.com/scorelab/TensorMap)

### [Project Wiki](https://github.com/scorelab/TensorMap/wiki)

### [Commits during GSoC 2018](https://github.com/scorelab/TensorMap/commits?author=suleka96)

### Pull Request links

* [PR 1](https://github.com/scorelab/TensorMap/pull/8)
* [PR 2](https://github.com/scorelab/TensorMap/pull/24)
* [PR 3](https://github.com/scorelab/TensorMap/pull/28)
* [PR 4](https://github.com/scorelab/TensorMap/pull/34)
* [PR 5](https://github.com/scorelab/TensorMap/pull/35)


### Work Summary

For GSoC 2019, I mainly worked on developing the Flask backend for TensorMap and I also worked on adding logic and UI to several frontend components.

### What was Covered

Backend 
 * Setup intial backend architecture
 * Implemented backend routes to handle auto generating of python Tensorflow (Keras) code according to the created model to:
   * Initialize environment for code auto generation according to experiment type (Binary Classification, Multiclass Classification, Regression)
   * Add new keras layer
   * Edit layer
   * Delete layer
   * Specify experiments configurations (number of epoch, loss function and etc)
   * Specify pre-processing information (features, labels, train and test splits and etc)
   * Download auto generated code file
   * Write validation for experiment type and model specific information
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
   * Specify features, labels and train percentage for experiment
   * Download edited CSV
 * Implement backend route to execute created model:
   * Create keras compatible JSON to genrate Keras model from recived layer informaation
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

As mentioned before, I mainly worked on the backend of the application thus, I have only included some screenshots of the frontend components I implemeted. 

Add data view
![](/relative/path/to/img.jpg?raw=true "Optional Title")

Visualize data view
![](/relative/path/to/img.jpg?raw=true "Optional Title")

### Reference

* [Tensorflow Keras](https://www.tensorflow.org/guide/keras)
* [React JS](https://reactjs.org)
* [Flask](https://flask.palletsprojects.com/en/1.1.x/)
* [material-table](https://material-table.com/#/)
* [SQLAlchemy](https://www.sqlalchemy.org)
