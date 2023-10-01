# PC Components Analysis Project

This project focuses on an in-depth analysis of datasets related to various PC components. The primary goal is to derive insightful visualizations and predictive models that can shed light on trends, correlations, and patterns concerning PC parts.

## Project Goals

- **Insightful Visualization**: Understand and visualize the distribution of various component features, trends over time, and identify correlations between different attributes.
- **Price Predictions**: Create machine learning models to forecast the future prices of PC components, enabling users to make informed decisions in a rapidly changing tech landscape.

## Datasets

- **CPU**: Contains details about various CPU models, their speeds, and respective prices.
- **GPU**: Lists different GPU models, their VRAM capacities, and prices.
- **RAM**: Details different RAM modules, their sizes in GB, and prices.
- **Storage (SSD)**: Contains data about various SSD models, their storage capacities, and prices.
- **Motherboard, Power Supply, and Cabinets**: These datasets offer details about other essential PC components.

## Detailed Steps & Results

### Data Exploration

- **Data Loading**: Imported datasets related to different PC components like CPU, GPU, RAM, and SSD.
- **Data Cleaning**: Addressed issues related to missing values, outliers, and incorrect data types.

### Insightful Visualization

- **Distribution Analysis**:
  - Visualized the distribution of prices for each component, highlighting the range and common price points.
  - Explored the distribution of performance metrics, such as CPU speed, GPU VRAM, RAM size, and SSD capacity.
- **Correlation Analysis**:
  - Used scatter plots and correlation coefficients to identify relationships between component prices and their performance metrics.
  - Found positive correlations between performance metrics and prices for most components, indicating that higher performance often comes at a premium.

### Price Predictions

- **Feature Engineering**:
  - Extracted relevant features from component descriptions, such as brand names.
  - Transformed and encoded categorical features for modeling.
- **Model Building & Evaluation**:
  - Used the Random Forest Regression model to predict performance metrics based on prices and other features for each component.
  - Evaluated models using metrics like RMSE and R-squared to understand the prediction accuracy and model fit.

## Conclusion

Through this project, we achieved a comprehensive understanding of the PC components market, recognizing significant trends and correlations. The predictive models built offer valuable insights into future price trends, aiding both consumers and businesses in making strategic decisions.
