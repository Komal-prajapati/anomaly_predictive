# Anomaly Detection for Predictive Maintenance

## Project Overview

This project aims to develop an anomaly detection system for predictive maintenance. The system uses a dataset containing various operational parameters of machinery to identify potential failures before they occur. The main focus is on detecting anomalies in the dataset using machine learning techniques.

## Dataset Description

The dataset contains the following columns:

- **UDI:** Unique identifier for each data entry.
- **Product ID:** Identifier for the product.
- **Type:** Type of the product or equipment.
- **Air temperature [K]:** Temperature of the air in Kelvin.
- **Process temperature [K]:** Temperature of the process in Kelvin.
- **Rotational speed [rpm]:** Rotational speed in revolutions per minute.
- **Torque [Nm]:** Torque in Newton-meters.
- **Tool wear [min]:** Tool wear time in minutes.
- **Machine failure:** Indicator of whether a machine failure occurred (binary).
- **TWF:** Tool Wear Failure (binary indicator).
- **HDF:** Heat Dissipation Failure (binary indicator).
- **PWF:** Power Failure (binary indicator).
- **OSF:** Overstrain Failure (binary indicator).
- **RNF:** Random Failure (binary indicator).

## Project Structure

```
├── data
│   └── your_dataset.csv     # The dataset file
├── notebooks
│   └── anomaly_detection.ipynb   # Jupyter notebook for analysis and model development
├── src
│   └── data_preprocessing.py    # Script for data preprocessing
│   └── anomaly_detection.py     # Script for anomaly detection model
├── README.md                    # Project description and instructions
├── requirements.txt             # Required packages and dependencies
└── visualization
    └── plots                    # Directory for storing plots and visualizations
```

## Getting Started

### Prerequisites

Ensure you have Python 3.x installed. Create a virtual environment and install the required packages using the following commands:



### Running the Project

1. **Clone the Repository:**


git clone https://github.com/your_username/anomaly-detection-predictive-maintenance.git
cd anomaly-detection-predictive-maintenance

2. **Prepare the Data:**

Ensure the dataset (`your_dataset.csv`) is placed in the `data` directory.

3. **Data Preprocessing:**

Run the data preprocessing script to clean and normalize the data.

```bash
python src/data_preprocessing.py
```

4. **Anomaly Detection:**

Run the anomaly detection script to train the model and identify anomalies.

```bash
python src/anomaly_detection.py
```

5. **Visualize the Results:**

Use the Jupyter notebook (`anomaly_detection.ipynb`) to explore the data, visualize anomalies, and further refine the model.

```bash
jupyter notebook notebooks/anomaly_detection.ipynb
```

## Methodology

1. **Load and Explore the Dataset:**
   - Import the dataset into a Pandas DataFrame.
   - Explore the structure and understand the columns.

2. **Data Preprocessing:**
   - Handle missing values.
   - Normalize numerical features.
   - Encode categorical variables.

3. **Anomaly Detection:**
   - Implement Isolation Forest for anomaly detection.
   - Train the model on the scaled features.
   - Predict anomalies and evaluate performance.

4. **Evaluation:**
   - Assess the performance using classification metrics like precision, recall, and F1-score.

5. **Visualization:**
   - Create visualizations to represent the data and detected anomalies.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments

Special thanks to the contributors and the community for their support and resources.


