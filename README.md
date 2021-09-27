# Toumetis Machine Learning Engineer Technical Interview

## Overview
The objective of this exercise is to build a prototype system that can be used for generating predictions of the operating mode for industrial assets.

Each machine was instrumented with a set of sensors and the data from these sensors has been collected and stored in a time-series database. 
Additionally, the operational mode has been labelled be an expert for each timestep. A csv dump of the database including the expert labels is available to support this task.

A data scientist has designed a deep learning solution in a notebook that performs well enough to be used in production. It is your job to take their work and use it as a basis for a prototype production system that can provide predictions given specific input data.

## Requirements
1. Carefully read through the jupyter notebook file that shows how the model was designed so you have a good understanding of the solution and why it was developed using this approach.
2. Develop production level solution for (at least a part of) the training and prediction functions for the model.
3. Develop a plan for productionising this model on a cloud platform, such as AWS. To give you some ideas for that you may wish to consider are (but by no means is this an exhaustive list) ... 
    - How the model will handle input data and serve predictions.
    - How the system performance will be monitored and the quailty of any outputs ensured.
    - Where any MLOps specific tools (e.g KubeFlow, MLflow, DVC, etc.) could be employed.

## Guidance
We understand that this is quite a lot to achieve in a reasonable amount of time and that the task is somewhat vague and very open ended. This is intentional as we wish to understand how you think about these type of open ended problems and your process for working through them with this forming the basis of our discussions at interview.  Consequently, it is very unlikely you will have a complete solution especially for part 2 above. In lieu of a complete solution a part solution detailed enough to demonstrate your competency with python would be sufficent here. Also, feel free to make whatever notes you feel appropriate and bring them to the interview. The interview itself will be discussion based so there is no need to share these with us, create a slide deck or anything like that.

## Questions and queries
If you have any questions or queries, please email Toumetis.

## Resources

### Data
Use the dataset in the `data/` directory. The **operational_mode** column is the target variable.

In the data directory there are three files. 
- raw_data.csv. This is the raw data for developing the model
- training_data.csv. The data used to train the model.
- validation_data.csv. The data used to validate model performance after training.
- test_data.csv. Hold out set for you to use for evaluating the model on unseen data. This contains data for 8 assets.

### Modelling
There is the notebook `model_development.ipynb` that you should use as a basis for your model.

### Misc
The conda environment file `environment.yaml` contains the packages and their versions used in the environment to develop the model.

## Submission
Please send your submission to Toumetis one full working day before your interview. Do not submit a pull request for this repository as other candidates may be able to view your solution.

