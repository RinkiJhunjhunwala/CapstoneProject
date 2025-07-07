# Project Architecture & Workflow

## Overview

This project is structured to simulate a real-time dynamic pricing system for urban parking lots. The workflow is as follows:

1. **Data Ingestion**
   - Data is loaded from a CSV file and/or streamed using Pathway to simulate real-time conditions.

2. **Feature Engineering**
   - Categorical features (traffic, vehicle type) are mapped to numerical values.
   - Time features are combined and formatted.

3. **Model 1: Baseline Linear Pricing**
   - Uses a simple linear function of occupancy to set the price.

4. **Model 2: Demand-Based Pricing**
   - Uses a multi-feature demand function and normalizes demand to set a dynamic price.

5. **Visualization**
   - Real-time price updates are visualized using Bokeh.

## Data Flow Diagram

![Architecture Diagram](architecture_diagram.png)

## Key Functions

- **demand_function()**: Computes demand using occupancy, queue, traffic, special day, and vehicle type.
- **dynamic_pricing()**: Calculates price based on normalized demand.
- **visualize_prices()**: Streams live price updates for each lot.

## Assumptions & Justifications

- Base price is $10, prices are clipped between $5 and $30.
- Demand coefficients are tuned for smooth, explainable price variation.
- No external ML libraries are used; all logic is implemented from scratch.

## Further Documentation

See [SummerAnalytics.ipynb](SummerAnalytics.ipynb) for complete code and inline explanations.

