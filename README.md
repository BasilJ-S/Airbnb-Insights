# Airbnb Insights

Machine learning analysis of Airbnb listings in Florence, Naples, and Venice to predict prices and review scores, identifying key amenities and factors affecting listing success.

## Overview

**Goal:** Predict listing prices and customer satisfaction (review scores) using property features and amenities.

**Dataset:** InsideAirbnb September 2023 data for three Italian cities (~5,000 listings, 75+ features).

**Methods:** XGBoost regression models for price and review prediction, with city-specific models.

## Key Components

**Feature Engineering:**
- Binary encoding for 95+ amenity types
- Distance to city center calculation
- Host verification and response metrics
- Property type and room type encoding

**Models:**
- Price prediction: XGBoost with log-transformed target
- Review prediction: XGBoost for overall rating and individual dimensions
- Separate models per city for localized predictions

## Key Findings

- Amenities (WiFi, kitchen, parking) significantly impact pricing
- Distance to city center strongly correlates with price
- Entire homes command higher prices than shared rooms
- Superhost status and response time influence reviews
- City-specific models outperform unified model

## Usage

Open `FinalProject_351.ipynb` in Google Colab, upload the InsideAirbnb CSV files for the three cities, and run cells sequentially.

**Technologies:** Python, pandas, scikit-learn, XGBoost, matplotlib, seaborn

## License

GNU General Public License v3.0 - see [LICENSE](LICENSE)

**CMPE 351 Final Project - Queen's University, Group 10**