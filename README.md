# Swiss Railways (SBB) Punctuality Analysis

## 🚆 Project Overview

Is the Swiss Railways Company (SBB) really on time? This project conducts a comprehensive analysis of train delays in the Swiss railway system, focusing on the Swiss Federal Railways (SBB). Using data pulled directly from data.sbb.ch, we investigate patterns, causes, and impacts of delays across various routes, times, and transportation types.

## 📊 Key Dataset Information

- **Date Collected**: 2024-05-06
- **Unique Train Stations**: 603
- **Total Records**: 63,050
- **Operator**: SBB
- **Modes of Transport**: 15 different types

## 🛠 Technologies Used

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- missingno
- folium

## 📚 Table of Contents

1. [Requirements](#requirements)
2. [Data Preparation](#data-preparation)
3. [Calculating Delay Probabilities](#calculating-delay-probabilities)
4. [Storing Results in a DataFrame](#storing-results-in-a-dataframe)
5. [Visualization](#visualization)
6. [Summary](#summary)
7. [Getting Started](#getting-started)
8. [Future Work](#future-work)
9. [License](#license)
10. [Contributing](#contributing)
11. [Contact](#contact)

## Requirements

Before you begin, ensure you have Python 3.x installed and the following packages:
```bash
pip install pandas numpy matplotlib seaborn missingno folium
```
To import these packages in your Python script or Jupyter notebook, use:

```bash
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import missingno as msno
import folium
```
## Data Preparation
The dataset contains information on various transport modes, stations, arrival and departure times, and delay status. Here's an overview of the train service types:

- R: Regio (Regional trains)
- IR: InterRegio (Regional express trains)
- S: S-Bahn (Suburban or metropolitan trains)
- RE: RegioExpress (Regional express services)
- ICE: InterCity Express (High-speed trains by Deutsche Bahn)
- IC: InterCity (Long-distance trains in Switzerland)
- EC: EuroCity (International long-distance trains)
- EXT: Extra (Additional or special services)
- TER: Transport Express Régional (Regional trains by SNCF)
- RJX: Railjet Express (High-speed trains by Austrian Federal Railways)
- NJ: Nightjet (Overnight sleeper trains)
- RB: RegionalBahn (Regional trains by Deutsche Bahn)
- TGV: Train à Grande Vitesse (High-speed trains by SNCF)
- SN: SNCF (French national railway company trains)
- ZUG: General term for "train" in German

## Calculating Delay Probabilities
We've explored probability calculations for delays based on:
- Transport mode
- Station
- Hour
- Minute
- These calculations offer a playful yet insightful look into the likelihood of delays.

Storing Results in a DataFrame
After calculating probabilities, we combine the results and store them in a DataFrame for efficient data analysis and visualization.

## Visualization
We employ various visualization techniques to provide a clear and comprehensive view of delay patterns:

- Missing Data Visualization: Using missingno to understand dataset completeness
- Correlation Analysis: Seaborn correlation matrix to explore relationships between variables
- Geographic Data Visualization: Interactive maps with folium to show station locations and delay probabilities
- Additional Visualizations: Bar charts and heatmaps using matplotlib and seaborn to illustrate delay patterns and insights

## Summary
This project focuses on understanding and visualizing delays in public transportation. Through detailed visualizations and analyses, we provide valuable insights into delay patterns. A separate notebook offers a fun exploration of delay probabilities for those interested.

The comprehensive understanding of transport delay patterns provided by this project can be used to improve prediction models and enhance the efficiency of public transport.

### 🚀 Getting Started
- Clone this repository
- Navigate to the project directory
- Install required packages:
- bash
- Code kopieren
- pip install -r requirements.txt
- Run the Jupyter notebooks

### 📈 Future Work
Deeper analysis of identified delay clusters
Integration of real-time data for predictive modeling
Expansion of the analysis to include multiple dates for trend identification

### 📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

### 🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

### 📬 Contact
For any questions or feedback, please open an issue in this repository.

### Enjoy your analysis and stay punctual! 🚂⏱️
