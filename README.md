# House Price Prediction ML Project

## Overview

This project aims to predict house prices based on various features using machine learning. The implementation follows proper coding conventions, design patterns, and strategies, while also integrating MLOps practices to ensure scalability, maintainability, and version control.

## Key Features

- **Machine Learning Model**: Predict house prices using regression models.
- **Design Patterns**: Implement design patterns such as Strategy, Factory, and Template for cleaner, more modular, and reusable code.
- **MLOps**: Incorporate MLOps practices for continuous integration, deployment, and monitoring of the machine learning models.

## Installation

Clone the repository:

```bash
git clone https://github.com/debarshee2004/prices-predictor-system.git
cd house-price-prediction
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Code Conventions and Patterns

### Coding Standards

- **PEP 8**: The codebase follows PEP 8 guidelines to ensure readability and consistency.
- **Docstrings**: Each function and class is documented with proper docstrings explaining their purpose and parameters.
- **Type Hinting**: We use Python's type hinting to make the code more explicit and catch potential issues during development.

### Design Patterns

1. **Factory Pattern**:
   - Used for creating instances of different models based on user configuration. This allows easy experimentation with multiple machine learning models.
   - File: `factory_design_pattern.py`
2. **Strategy Pattern**:
   - Used to dynamically switch between different preprocessing and feature engineering techniques depending on the dataset.
   - File: `strategy_design_pattern.py`
3. **Template Method Pattern**:
   - Defines the skeleton of the model training process, leaving the specifics of preprocessing, feature selection, and training to subclasses.
   - File: `template_design_pattern.py`

### Strategies

- **Separation of Concerns**: All functionalities (data processing, model training, evaluation) are separated into individual modules to ensure modularity and reusability.
- **Parameterization**: Hyperparameters and configurations are stored in `config.yaml` to allow easy adjustments and experimentation without changing the code.

## MLOps Practices

### Version Control

We use Git for version control of both the code and the models.

### Experiment Tracking

MLflow is integrated to track experiments, hyperparameters, and metrics during the model training process. Each model's performance is logged and can be compared easily.

### CI/CD Pipeline

We implement a CI/CD pipeline using GitHub Actions to automatically run unit tests and deploy the latest model after a successful merge into the main branch.

### Model Registry

Models are stored in an MLflow model registry, which allows for versioning and easier rollback in case of issues.

### Deployment

Once a model is trained, it can be deployed to production via Docker, ensuring a consistent environment across all stages from development to production.

## Contribution Guidelines

- Follow PEP 8 guidelines.
- Ensure all functions have clear docstrings.
- Add unit tests for any new functionality.
- Ensure all CI/CD checks pass before making a pull request.

## License

This project is licensed under the MIT License.
