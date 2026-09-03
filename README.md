# VayuDrishti
### AI/ML-Based Tropical Cyclone Identification, Classification & Prediction System

> **Smart India Hackathon 2026 — Problem Statement: SIH26070**

VayuDrishti is an Artificial Intelligence and Machine Learning based platform designed to analyze **multi-source satellite data** for the identification, classification, tracking, and prediction of tropical cyclone patterns.

The system aims to transform large volumes of satellite observations into meaningful cyclone intelligence through an end-to-end pipeline covering **data acquisition, preprocessing, AI/ML analysis, prediction, backend services, and an interactive visualization dashboard**.

---

## Table of Contents

- [About VayuDrishti](#-about-vayudrishti)
- [Problem Statement](#-problem-statement)
- [Problem Overview](#-problem-overview)
- [Our Solution](#-our-solution)
- [Key Objectives](#-key-objectives)
- [Key Features](#-key-features)
- [System Architecture](#-system-architecture)
- [Overall Workflow](#-overall-workflow)
- [Data Sources](#-data-sources)
- [AI/ML Pipeline](#-aiml-pipeline)
- [Cyclone Detection](#1-cyclone-detection)
- [Cyclone Classification](#2-cyclone-classification)
- [Cyclone Tracking](#3-cyclone-tracking)
- [Cyclone Prediction](#4-cyclone-prediction)
- [Technology Stack](#-technology-stack)
- [Project Structure](#-project-structure)
- [Frontend](#-frontend)
- [Backend](#-backend)
- [Machine Learning](#-machine-learning)
- [Database](#-database)
- [Deployment](#-deployment)
- [Installation & Setup](#-installation--setup)
- [Environment Variables](#-environment-variables)
- [API Overview](#-api-overview)
- [Model Evaluation](#-model-evaluation)
- [Expected Output](#-expected-output)
- [Development Roadmap](#-development-roadmap)
- [Future Scope](#-future-scope)
- [Team](#-team)
- [Contribution](#-contribution)
- [License](#-license)

---

# About VayuDrishti

Tropical cyclones are among the most destructive natural hazards, capable of causing severe impacts on human life, infrastructure, agriculture, coastal regions, and ecosystems.

Timely identification and accurate prediction of cyclone development, movement, and intensity are therefore important for disaster management, emergency response, coastal safety, and risk assessment.

Modern Earth-observation satellites continuously generate large amounts of atmospheric and surface data. However, extracting useful information from this data at scale is challenging because satellite observations can differ in:

- Spatial resolution
- Temporal resolution
- Spectral characteristics
- Data format
- Geographic coverage
- Observation frequency

**VayuDrishti** aims to address this challenge by developing an AI/ML-powered pipeline capable of processing multi-source satellite observations and extracting cyclone-related information automatically.

The platform combines:

```text
Satellite Data
      ↓
Data Acquisition
      ↓
Data Processing
      ↓
AI / ML Analysis
      ↓
Detection
      ↓
Classification
      ↓
Tracking & Prediction
      ↓
Backend Services
      ↓
Interactive Dashboard
```
# Problem Statement
Develop an Artificial Intelligence (AI) / Machine Learning (ML) based system for identification, classification, and prediction of different tropical cyclone patterns using multi-source satellite data.

**Core Challenge**

The objective is to develop an intelligent system that can process satellite observations from multiple sources and use AI/ML techniques to:

- Identify tropical cyclone formations
- Recognize cyclone-related patterns
- Classify detected cyclone systems
- Track cyclone movement
- Predict future cyclone trajectory
- Analyze intensity-related characteristics
- Present the results through an accessible visualization platform


# Problem Overview

**Why is this problem challenging?**
1. Large Volumes of Satellite Data

Satellite platforms continuously generate huge quantities of Earth-observation data.

Manual inspection of this data can be:

- Time-consuming
- Difficult to scale
- Dependent on expert interpretation
- Computationally expensive

2. Multi-Source Data

Different satellites provide different types of observations.

These may include:

- Visible imagery
- Infrared imagery
- Water-vapor imagery
- Microwave observations
- Ocean observations
- Atmospheric observations

Combining these heterogeneous observations into a unified pipeline presents a significant data-engineering challenge.

3. Cyclone Identification

A tropical disturbance must be distinguished from other atmospheric systems.

The system should learn visual and spatial patterns associated with cyclone formation and identify potential cyclone systems automatically.

4. Cyclone Classification

Cyclones can exhibit different structural characteristics and intensity levels.

An AI/ML model can assist in classifying detected cyclone systems according to learned patterns and available ground-truth categories.

5. Cyclone Tracking

Cyclones evolve continuously over time.

Successive satellite observations can be used to estimate the movement of a cyclone and generate its historical track.

6. Cyclone Prediction

Prediction requires understanding both the current state and historical evolution of the cyclone.

Potential prediction targets include:

- Future latitude
- Future longitude
- Direction of movement
- Intensity
- Wind speed
- Central pressure

# Our Solution
VayuDrishti proposes an end-to-end AI/ML pipeline for tropical cyclone analysis.
![alt text](<Screenshot 2026-09-03 215600.png>)

# Key Objectives
1. Multi-Source Data Integration

Integrate satellite observations from multiple publicly available sources into a unified data pipeline.

2. Automated Data Preprocessing

Clean, normalize, align, and transform raw satellite observations into machine-learning-ready datasets.

3. Cyclone Identification

Automatically identify cyclone formations and cyclone-like patterns from satellite imagery.

4. Cyclone Classification

Classify detected cyclones according to relevant structural and intensity characteristics.

5. Cyclone Tracking

Track cyclone movement across successive satellite observations.

6. Cyclone Prediction

Predict future cyclone trajectory and potentially intensity-related parameters using temporal AI/ML models.

7. Visualization

Provide cyclone information through an interactive web dashboard.

8. Decision Support

Provide useful cyclone information that can assist disaster-management and monitoring activities.

# Key Features
**Multi-Source Satellite Data**

Support multiple satellite and auxiliary data sources through a unified processing pipeline.

**AI-Based Cyclone Detection**

Automatically identify potential cyclone systems from satellite observations.

**Cyclone Classification**

Classify detected systems according to learned cyclone patterns and available intensity categories.

**Cyclone Tracking**

Track cyclone movement using sequential satellite observations.

**Future Position Prediction**

Estimate the future trajectory of a cyclone using historical and current observations.

**Intensity Analysis**

Analyze cyclone intensity-related characteristics and provide predictions where supported by the trained model.

**Interactive Map**

The dashboard can display:

- Current cyclone position
- Historical trajectory
- Predicted trajectory
- Intensity information
- Geographic coordinates
- bservation timestamps

**Analytics Dashboard**

The dashboard can provide:

- Cyclone statistics
- Historical cyclone information
- Model predictions
- Confidence scores
- Time-series information
- Satellite imagery
**Alert System**

The platform can be extended to generate alerts when potentially significant cyclone conditions are detected or predicted.

Potential notification channels:

- Web notifications
- Email
- SMS
- Push notificatio