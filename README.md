# Predicting Patient Charges 🤖💰

![GitHub Repo Stars](https://img.shields.io/github/stars/DuhaPr1/predicting-patient-charges?style=social) ![GitHub Issues](https://img.shields.io/github/issues/DuhaPr1/predicting-patient-charges) ![GitHub License](https://img.shields.io/github/license/DuhaPr1/predicting-patient-charges)

Welcome to the **Predicting Patient Charges** repository! This project aims to provide a comprehensive end-to-end MLOps solution for predicting patient insurance charges using machine learning. Built with cutting-edge technologies, this project covers everything from data processing to deployment in a live environment.

## Table of Contents

- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Testing](#testing)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)
- [Links](#links)

## Project Overview

The **Predicting Patient Charges** project implements a machine learning pipeline that predicts the insurance charges for patients based on various features. The project uses PyCaret for automated machine learning, simplifying the model training and selection process. A Flask web application serves as the front end, allowing users to interact with the model seamlessly.

This project includes:

- **Data Preprocessing**: Clean and prepare the data for modeling.
- **Feature Engineering**: Create meaningful features to improve model performance.
- **Model Training**: Utilize PyCaret to automate the training of multiple models.
- **Web Application**: A user-friendly interface built with Flask.
- **Containerization**: Use Docker to package the application for easy deployment.
- **CI/CD Pipeline**: Implement GitHub Actions for continuous integration and deployment.
- **Cloud Deployment**: Host the application on Azure for scalability.

You can download the latest version of the project from the [Releases section](https://github.com/DuhaPr1/predicting-patient-charges/releases).

## Technologies Used

This project leverages a variety of technologies to deliver a robust solution:

- **Python**: The primary programming language used for data analysis and model building.
- **PyCaret**: A low-code machine learning library that simplifies the model training process.
- **Flask**: A lightweight web framework for building the web application.
- **Docker**: Containerization technology that allows the application to run consistently across different environments.
- **Azure**: Cloud platform for deploying the application.
- **GitHub Actions**: CI/CD tool for automating the deployment process.

## Installation

To set up the project locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/DuhaPr1/predicting-patient-charges.git
   cd predicting-patient-charges
   ```

2. **Install dependencies**:
   Create a virtual environment and activate it:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

   Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up environment variables**:
   Create a `.env` file in the root directory and add the necessary configuration settings.

4. **Run the application**:
   Start the Flask server:
   ```bash
   python app.py
   ```

The application will be available at `http://127.0.0.1:5000`.

## Usage

Once the application is running, you can access it through your web browser. The user interface allows you to input patient data, and it will return the predicted insurance charges based on the trained model.

### Input Fields

- **Age**: Patient's age.
- **Gender**: Patient's gender.
- **BMI**: Body Mass Index.
- **Children**: Number of children/dependents covered by insurance.
- **Smoker**: Whether the patient is a smoker (Yes/No).
- **Region**: The region where the patient resides.

After entering the data, click on the "Predict" button to see the estimated charges.

## Features

- **Automated Model Selection**: Uses PyCaret to automatically select the best model based on the data.
- **User-Friendly Interface**: The Flask web app provides an intuitive interface for users.
- **Docker Support**: Easily deploy the application using Docker.
- **Continuous Integration**: Automatically run tests and deploy the application using GitHub Actions.
- **Comprehensive Documentation**: Detailed documentation is available to help users understand the project.

## Testing

The project includes a set of tests to ensure that the application works as expected. To run the tests, use the following command:

```bash
pytest tests/
```

This will execute all the tests located in the `tests` directory. Make sure to have all dependencies installed before running the tests.

## Deployment

The application can be deployed on Azure using Docker. Follow these steps to deploy:

1. **Build the Docker image**:
   ```bash
   docker build -t predicting-patient-charges .
   ```

2. **Run the Docker container**:
   ```bash
   docker run -p 80:5000 predicting-patient-charges
   ```

3. **Push to Azure**:
   Use Azure CLI to push the Docker image to your Azure Container Registry and deploy it to Azure App Service.

## Contributing

We welcome contributions to improve this project. If you have suggestions or improvements, please fork the repository and submit a pull request. Make sure to follow the contribution guidelines.

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add new feature'`).
5. Push to the branch (`git push origin feature/YourFeature`).
6. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Links

For more information, check out the [Releases section](https://github.com/DuhaPr1/predicting-patient-charges/releases) for the latest updates and downloadable files.