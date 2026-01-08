# Offline Wood Tracking System (Master Thesis)

> **Company:** PEPPS <br>
> **Project:** Wood Tracking System (dWTS) <br>
> **Role:** R&D Software Engineer (Master Thesis) <br>
> **Status:** Active <br>
> **Timeline:** 2025-2026 <br>
> **Tech Stack:** React, PWA, Python, YOLOv8, ONNX Runtime

## Overview

This project focuses on the development of an **offline-first Progressive Web App (PWA)** to digitize the tracking of harvested logs in the rainforests of Guyana. The system replicates the manual process of measuring log diameters using computer vision, running entirely on low-end Android devices without internet access.


## Technical Implementation

*   **Core Challenge:** Implementing real-time object detection and storage on entry-level mobile devices with **zero connectivity**.
*   **AI Model:** Fine-tuned **YOLOv8-nano** segmentation model to detect logs and physical reference tags.
*   **Data Strategy:** Leveraged aggressive **data augmentation** (geometric & photometric) to train a robust model from a small dataset of 26 images.
*   **Architecture:** The model was exported to **ONNX** format and run directly in the browser using **ONNX Runtime Web**, enabling a completely offline workflow.

## Project Poster

For a detailed breakdown of the methodology, algorithms, and results, please refer to the project poster below.

![Thesis Poster](./assets/poster.jpg)


## Confidentiality Notice

> **Note:** The complete source code for this project is private. This repository serves strictly as a portfolio showcase.
