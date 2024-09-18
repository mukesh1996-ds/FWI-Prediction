# Algeria Fire Prediction

## Project Overview
This project aims to predict fire occurrences in Algeria based on various environmental and weather-related factors. The main target variable for prediction is the **Fire Weather Index (FWI)**, a numerical indicator used to estimate the potential for fire ignition and spread.

The FWI system is widely used for fire weather monitoring, and it's part of the **Canadian Forest Fire Weather Index System**. The model developed here will analyze historical data from Algeria, specifically targeting regions prone to wildfires, and provide insights and predictions to help in early fire detection and prevention.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Target Variable](#target-variable)
- [Modeling Approach](#modeling-approach)
- [Usage](#usage)
- [Installation](#installation)
- [Contributing](#contributing)
- [License](#license)

## Dataset
The dataset consists of various environmental and meteorological factors collected from regions in Algeria that are prone to forest fires. These factors include:
- Temperature
- Relative Humidity
- Wind Speed
- Rainfall
- Drought Code (DC)
- Duff Moisture Code (DMC)
- Initial Spread Index (ISI)

### Target Variable: Fire Weather Index (FWI)
The **Fire Weather Index (FWI)** is the main target variable for this prediction task. It is a combination of different weather components that estimate fire risk. A higher FWI indicates a higher likelihood of fire ignition and spread.

## Modeling Approach
The project follows a standard machine learning pipeline:
1. **Data Preprocessing**: Handling missing values, encoding categorical features, and scaling numerical values.
2. **Feature Engineering**: Adding domain-specific features to improve model performance.
3. **Model Selection**: Training different machine learning models (Random Forest, Gradient Boosting, etc.) to predict FWI.
4. **Evaluation**: Evaluating models based on metrics like RMSE, MAE, and R-squared.

## Usage
To use this project, follow these steps:

1. Clone this repository:
    ```bash
    git clone https://github.com/yourusername/algeria-fire-prediction.git
    cd algeria-fire-prediction
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the preprocessing and training scripts:
    ```bash
    python preprocess.py
    python train_model.py
    ```

4. Make predictions on new data:
    ```bash
    python predict.py --input data/new_input.csv
    ```

## Installation
1. Install [Python](https://www.python.org/downloads/) (version 3.7 or higher).
2. Install dependencies by running:
    ```bash
    pip install -r requirements.txt
    ```

## Contributing
Contributions to this project are welcome! If you'd like to improve the model or add new features, please fork the repository and create a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
