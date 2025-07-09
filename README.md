# dynamic-parking-pricing
# 🚗 Dynamic Pricing for Urban Parking Lots

Capstone Project – Summer Analytics 2025  
Organized by the Consulting & Analytics Club, IIT Guwahati × Pathway

---

## 📌 Project Overview

Urban parking spaces are a limited resource. Static pricing often leads to either overcrowding or underutilization. This project implements a **dynamic pricing engine** for 14 urban parking lots using real-time data and basic economic theory, with the goal of improving utilization and reducing congestion.

---

## 🛠️ Tech Stack

- **Languages**: Python (NumPy, Pandas)
- **Real-time Simulation**: Pathway
- **Visualization**: Bokeh
- **Notebook Environment**: Google Colab

---

## 🧠 Models Implemented

### 🔹 Model 1 – Baseline Linear Model
- Price increases linearly with occupancy:

### 🔹 Model 2 – Demand-Based Pricing
- A custom demand function incorporates:
- Occupancy rate
- Queue length
- Traffic condition
- Special day indicator
- Vehicle type

- Price is adjusted as:


### 🔹 Model 3 – Competitive Pricing (Optional)
- Adds spatial intelligence by factoring in:
- Nearby parking lot prices (calculated via latitude/longitude)
- Suggests rerouting if current lot is full and nearby lots are cheaper

---

## 🔁 Real-Time Simulation with Pathway

- **Streaming Ingestion**: Simulated delay-based data feed
- **Real-time Output**: Pricing decisions emitted continuously
- **Pathway Features Used**:
- Time-preserving streaming pipeline
- Real-time feature updates

---

## 📊 Visualizations

Generated using **Bokeh**, including:
- Real-time line charts of price changes per parking lot
- Competitor price comparison plots

---

## 📂 Repository Structure


---

## 📈 Architecture Diagram

```mermaid
graph TD
    A[Input Stream - CSV Data] --> B[Pathway Ingestion Engine]
    B --> C[Feature Extraction & Preprocessing]
    C --> D[Model 1, 2, 3 Pricing Engines]
    D --> E[Price Output Stream]
    E --> F[Bokeh Real-Time Visualization]

  
