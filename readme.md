# Sparkify

Capstone Project of the udacity Data Scientist nanodegree

## Project description

Sparkify is a music streaming service which features a paid and an unpaid level. In unpaid level it is supposed to rolling advertisements.
Users can upgrade to paid level and downgrade to free level and cancel their membership on the service.
Goal of the project is predicting whether a user is about to cancel so that marketing can step in with something to prevent that from
happening.

The student shall get to know the big data map-reduce-platform spark. 12 GB of clickstream data of the Sparkify website is delivered
as a json file to be processed with spark into derived features which a model can be trained on a per user basis.

## Files

*Sparkify_Feature_Creation.ipynb* is a jupiter notebook implementing the steps from the raw data to the derived features.

*Sparkify_MOdel.ipynb* starts with the derived user features trying out different ML models to predicting the churn of users

*bootstrap.sh* setup script for AWS EMR

## Utilities used

The *Sparkify_Feature_Creation.ipynb* was developed on AWS EMR. For having the needed packages evailable the *bootstrap.sh* was included in the cluster setup
as bootstrap script as well as a script-runner.jar step.

As after feature creation the data is no longer considered "big" the model development was carried out on a laptop in a jupyter/all-spark-notebook docker container.

## Blog post

More information about the models derived can be found in this blogpost: https://medium.com/@jan.krueger/4241ba1555d5
