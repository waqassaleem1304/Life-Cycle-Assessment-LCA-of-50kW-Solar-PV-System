# Life Cycle Assessment (LCA) of 50kW Solar PV System

## 📖 Project Overview
This project quantifies the environmental impact of a **50kW Solar Photovoltaic (PV) System** throughout its lifespan. 

The tool tracks Greenhouse Gas (GHG) emissions from **Cradle-to-Grave** (Raw Materials to End-of-Life Recycling) to identify environmental hotspots and calculate the social cost of carbon.

## ⚙️ Methodology
The analysis processes inventory data using Python to compute Carbon Footprint ($CO_2e$) and Carbon Pricing.

### 1. Emission Logic
Emissions are calculated per activity using standard Emission Factors (EF):
$$\text{Emissions (ton)} = \frac{\text{Quantity} \times \text{EF}}{1000}$$

### 2. Assessment Stages
* **Raw Materials:** Polysilicon, Glass, Aluminum, Copper.
* **Manufacturing:** PV Modules, Inverters.
* **Logistics:** Transportation & Installation.
* **Operation:** Grid losses & Maintenance.
* **End-of-Life:** Recycling credits (Negative emissions).

## 📊 Key Results
Analysis identifies **Raw Material Extraction** as the highest impact stage.

| Parameter | Calculated Value |
| :--- | :--- |
| **Total Lifetime Emissions** | `63.56 ton CO2e` |
| **Net Carbon Saved (Recycling)** | `4.00 ton CO2e` |
| **Social Carbon Cost** | `4,004.31 €` (@63€/ton) |
| **Primary Hotspot** | `Polysilicon Production` (41.25 ton) |

## 📈 Visualization

### Figure 1: Emissions by Life Cycle Stage
<img width="841" height="614" alt="image" src="https://github.com/user-attachments/assets/01e14f8d-418f-464d-8a20-5c4d517abf85" />

> *Bar graph indicating Raw Materials as the dominant emission source.*

### Figure 2: Top 5 Activities
<img width="714" height="658" alt="image" src="https://github.com/user-attachments/assets/6975f7f3-5fdd-4b41-bab1-e569c3dac553" />

> *Pie chart breakdown showing Polysilicon and Module Manufacturing as key contributors.*

## 🛠️ Tech Stack
* **Python:** `Pandas` (Data Processing), `Seaborn` (Visualization).
* **Input/Output:** Excel (`.xlsx`).

---
