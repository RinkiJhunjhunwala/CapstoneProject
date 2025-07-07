# Dynamic Pricing for Urban Parking Lots

**Capstone Project – Summer Analytics 2025**  
Consulting & Analytics Club × Pathway

## 🚀 Overview

This project implements a real-time, data-driven dynamic pricing engine for 14 urban parking lots. The goal is to optimize parking utilization and revenue using machine learning and economic principles, leveraging real-time data streams and Pathway for live simulation.

## 🛠️ Tech Stack

- **Python 3**
- **Pandas** & **NumPy** (data processing, modeling)
- **Pathway** (real-time data streaming)
- **Bokeh** (visualization)
- **Google Colab** (development environment)
- **GitHub** (version control, documentation)

## 🏗️ Architecture Diagram
![architecture_image](https://github.com/user-attachments/assets/b4f4630b-2fee-44c8-b75e-c627ccf8a0b7)


## 📚 Project Architecture & Workflow

1. **Data Ingestion:**  
   - Load data from CSV or real-time stream using Pathway.
2. **Feature Engineering:**  
   - Clean data, map categorical variables, create time features.
3. **Model 1 – Baseline Linear Pricing:**  
   - Price increases linearly with occupancy.
4. **Model 2 – Demand-Based Pricing:**  
   - Price set by a demand function using occupancy, queue, traffic, special events, vehicle type.
5. **Real-Time Simulation:**  
   - Pathway simulates real-time data flow and pricing updates.
6. **Visualization:**  
   - Bokeh provides real-time price plots for each parking lot.

## 📖 Documentation

- [architecture.md](architecture.md): Detailed explanation of the project architecture and workflow.
- [SummerAnalytics.ipynb](notebook.ipynb): Well-commented Colab notebook with all code, models, and visualizations.
- [report.pdf](report.pdf): (Optional) Project report with explanations and justifications.

## 📋 How to Run

1. Clone this repository:
2. Open `SummerAnalytics.ipynb` in Google Colab.
3. Follow the instructions in the notebook to run each cell.


