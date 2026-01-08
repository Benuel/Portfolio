# Crowd Estimation for Festivals

> **Company:** Couleur Café <br>
> **Project:** Crowd Estimation for Festivals <br>
> **Role:** Co-Author / Developer <br>
> **Status:** Active <br>
> **Timeline:** 2025 <br>
> **Tech Stack:** Python, Flask, SocketIO, JS, Tailwind CSS, PyTorch, OpenCV

> [🇫🇷 Lire en Français](./README.fr.md)

## Overview

**Crowd Estimation for Festivals** is a real-time web application designed to visualize crowd density and count across multiple festival locations. Optimized for large screen displays in control rooms, it helps safety teams monitor attendee flow and density in real-time.


## Features

![Screenshot](assets/Screenshot.png)

*   **Real-Time Monitoring:** Displays live total people count and density (people/m²) for multiple stages.
*   **Visual Verification:** Shows the actual processed image alongside the data for instant visual confirmation.
*   **Smart Alerts:** Uses configurable color thresholds (Green/Orange/Red) to instantly highlight potential overcrowding.
*   **Time Navigation:** Allows operators to browse historical data and review past crowd states.
*   **Live Mode:** Automatically updates with fresh data as soon as new analysis arrives.



## Technical Architecture

The system operates as a pipeline:
1.  **Ingestion:** Extracts RTSP video streams from festival security cameras.
2.  **Analysis:** A Python-based AI model (leveraging the **APGCC** pretrained project) processes images to detect heads and estimate density maps.
3.  **Serving:** A Flask backend broadcasts updates via WebSockets (Flask-SocketIO) to the frontend.
4.  **Display:** A reactive dashboard built with HTML5 and Tailwind CSS renders the data.


## Confidentiality Notice

> **Note:** The complete source code, detailed AI model configurations, and deployment scripts are not publicly available. This repository serves strictly as a portfolio showcase of the product and its features.
