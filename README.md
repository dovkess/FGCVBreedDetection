# FGCV Breed Detection

A project to detect and classify dog breeds from images collected and stored in Google Drive. 
The pipeline consists of three main stages:

1. Collect and store images in Drive
2. Run the YOLO detection pipeline to find and crop dog instances
3. Run the trainDogs pipeline to train a classifier on the cropped dog images for breed classification

This repository contains the pipelines and helper scripts used to run the full workflow.

## Overview

- Images: store raw images in your Google Drive (or other mounted drive). The exact path is configurable in the pipeline scripts
- YOLO pipeline: runs object detection to locate dogs in images, producing cropped images and detection annotations.
- trainDogs pipeline: uses the outputs from the YOLO pipeline (cropped dog images and labels/annotations) to train a breed classification model.

## Quickstart

Best to use in google Colab
