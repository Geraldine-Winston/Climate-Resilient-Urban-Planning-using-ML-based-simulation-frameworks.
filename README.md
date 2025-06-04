# Climate-Resilient Urban Planning using ML-based Simulation Frameworks

This project develops a machine learning-based simulation framework to recommend urban planning designs that enhance climate resilience. The model predicts resilience indices based on urban parameters like green space, building density, and water infrastructure.

## Project Overview

- **Input**: Urban features such as green space percentage, building density, road network density, water infrastructure score, and population density.
- **Model**: A machine learning regression model (Random Forest) trained to predict a resilience index.
- **Output**: Recommended urban designs that maximize resilience to climate risks such as floods, heatwaves, and air quality deterioration.

## Project Structure

```
📁 Climate-Resilient-Urban-Planning-ML
├── generate_urban_data.py                # Code to simulate urban planning data
├── model_training.py                      # Code to train ML model
├── recommend_design.py                    # Code for generating urban design recommendations
├── full_urban_planning_data.xlsx          # Full synthetic dataset
├── urban_planning_recommendations.xlsx    # Top recommended urban plans
├── README.md                               # Project documentation
├── requirements.txt                        # Python dependencies
└── .gitignore                               # Files to ignore in version control
```

## Requirements

Install all necessary dependencies using:

```bash
pip install -r requirements.txt
```

**Dependencies:**

```
pandas
numpy
scikit-learn
openpyxl
```

## How to Run

1. Generate the synthetic urban planning data:

```bash
python generate_urban_data.py
```

2. Train the ML model:

```bash
python model_training.py
```

3. Generate recommendations for urban planning designs:

```bash
python recommend_design.py
```

4. Outputs:
   - **`full_urban_planning_data.xlsx`**: Complete urban planning dataset with resilience indices.
   - **`urban_planning_recommendations.xlsx`**: Top recommended urban planning configurations.

## Dataset Example

```csv
green_space_percentage,building_density,road_network_density,water_infrastructure,population_density,resilience_index
45.2,6.5,12.3,0.72,4500,78.5
30.1,8.2,15.7,0.65,7000,69.8
...
```

## Model Performance

The Random Forest model achieves:
- **Test MSE**: 20.47
- **Test R² Score**: 0.87

## Acknowledgements

- Urban resilience principles inspired by global best practices.
- Future extensions can integrate real-world urban GIS datasets and climate scenario modeling.

## Author

**Ayebawanaemi Geraldine Winston**

