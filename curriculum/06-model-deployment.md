# Model Deployment

1. [General](#1-general)
2. [Curriculum](#2-curriculum)
3. [Topics Not Covered](#3-topics-not-covered)

## 1 General

This specialization should cover the topics required for delivering the Capstone and introduce students to model deployment in real life.


## 2 Curriculum

| BLU   | Name                     | Status | Content           |
| ----- | ------------------------ | ------ | ----------------- |
| BLU13 | Basic Model Deployment   | Draft  | [Content](#blu13) |
| BLU14 | Deployment in Real World | Draft  | [Content](#blu14) |
| BLU15 | Model CSI                | Draft  | [Content](#blu15) |

## Contents

### BLU13

#### Basic Model Deployment

How to make a scikit model available to the world, serve prediction requests and receive ground truth data for your prediction (so that you can retrain your model later on).

##### Main topics

1. Serializing and deserializing scikit learn models
2. Flask app
3. Heroku model deployment

##### Detailed curriculum

1. Serializing and deserializing scikit learn models

   1. Defining the data journey: train, serialize, predict
   2. Predict from JSON
   3. Train and serialize
   4. Deserialize and predict

2. Flask app
   1. Introduction to Flask
   2. Create a basic server
   3. Keep track of predictions (cf. Data modelling)

3. Heroku model deployment

   1. Introduction to Heroku
   2. Heroku CLI
   3. App deployment
   4. Endpoint testing
      1. Test predictions with predict/
      2. Test db storage with retrieve/
   5. Common problems

### BLU14

#### Deployment in Real World

How to deploy a model in the wild.

##### Main topics

1. Formalizing client requirements
2. Dealing with unexpected inputs
3. Uptime and surviving failures
4. (Optional) Heroku guides

##### Detailed curriculum

1. Formalizing client requirements

    1. Expectation vs reality when dealing with clients
    2. Converting business requirements to technical metrics
    3. Fairness & privacy requirements, model prioritization
    4. Technical architecture diagram (e.g. connections between database, webserver, endpoints, etc.)
    5. Threshold tuning meets business requirements

2. Dealing with unexpected inputs

    1. Unexpected values
    2. Data selection: relevant data, denoysing
    3. Data structure definition

3. Uptime and surviving failures

    1. Potential errors (e.g. formats, values, missing data)
    2. Input validation
    3. Application structure
    4. Logging, Metrics, Monitoring and Alerting
    5. Testing (unit test, test-driven development)

4. Heroku guides (Optional for students, in markdown)
   1. Restart the app
   2. Reset the database
   3. Checking logs
   4. Retrieiving data (e.g. DBeaver, dataclip feature in Heroku)

### BLU15

#### Model CSI

How to diagnose, debug and redeploy an existing model.

#### Main topics

1. Model investigation
2. Retraining and Redeployment

##### Detailed curriculum

1. Model investigation

   1. Model diagnosing
   2. Need for retraining
      1. Drifts: data (input), label (outputs) and concept (relation)
      2. Robustness
      3. Ground truth unavailability

   3. Measuring performance over time
      1. Measuring data drifts
      2. Measuring model drifts

   4. Fixing model problems

2. Retraining and Redeployment

   1. Model retraining

      1. Manual, periodic and continuous strategies
      2. Choosing retraining data

   2. Model redeployment

        1. Identifying potential issues and risks
        2. Production errors and logging
        3. Preemptive vs reactive deployments

## 3 Topics Not Covered

*WIP*
