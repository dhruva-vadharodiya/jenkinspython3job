# jenkinspython3job
# Jenkins Upstream & Downstream Pipeline Demo

## Overview

This repository demonstrates the basic concept of **Upstream and Downstream Jobs** using Jenkins. It simulates a simple CI workflow where each stage is executed as an independent Jenkins job. After one job completes successfully, Jenkins automatically triggers the next job.

## Repository Structure

### Python Repository

* `dev.py` – Simulates the Development stage.
* `test.py` – Simulates the Testing stage.
* `prod.py` – Simulates the Production Deployment stage.


## Jenkins Workflow

```
GitHub Repository
        │
        ▼
Development Job
        │
        ▼
Testing Job
        │
        ▼
Production Job
```

Each Jenkins job is configured with **Build Other Projects** as a post-build action. When the Development job finishes successfully, it automatically triggers the Testing job. Similarly, the Testing job triggers the Production job after a successful build.

## What I Learned

* Creating Jenkins Freestyle Jobs
* Connecting Jenkins with GitHub
* Executing Python and Java programs from Jenkins
* Configuring Build Steps
* Understanding Upstream and Downstream Jobs
* Triggering jobs automatically after a successful build
* Building a simple Continuous Integration workflow

## Technologies Used

* Jenkins
* GitHub
* Python
* Java
* Git

## Purpose

The purpose of this repository is to understand how Jenkins automates a multi-stage workflow by linking jobs together using the Upstream and Downstream job concept. This serves as a foundation for learning more advanced CI/CD pipelines.
