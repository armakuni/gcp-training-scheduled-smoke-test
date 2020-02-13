# Scheduled GCP Training Microservice Smoke Test
This project is used for only executing the smoke tests in scheduled interval.

The [cloudbuild.yaml](cloudbuild.yaml) pipeline has two steps i.e.,
* First step for storing the variables in the container volume mount.
* Second step for executing the smoke tests.

This repository should be connected to the cloud build trigger and execution to be scheduled for every 5 min using Cloud Scheduler.

## Execute smoke test in cloud build using local trigger
```bash
gcloud builds submit
```