# Brain Tumour Classification API

This repository provides a Python-based API for detecting brain tumours from medical images. The solution uses deep learning models to identify tumours and includes an interactive notebook for running the detection pipeline.

## Table of Contents

1. [Overview](#overview)
2. [Features](#features)
3. [Setup and Installation](#setup-and-installation)
4. [Usage](#usage)
5. [Model and Methodology](#model-and-methodology)
6. [Results](#results)
7. [Contributing](#contributing)
8. [License](#license)

## Overview

Brain tumours are serious medical conditions requiring early detection for effective treatment. This project provides an automated approach to detecting brain tumours from medical imaging data using a convolutional neural network (CNN)-based classifier. The API is implemented in Python and uses Jupyter Notebook for demonstration.

## Features

- **Deep Learning-based Detection**: Utilizes CNNs for identifying tumours in MRI scans.
- **Interactive Notebook**: Includes a notebook for experimenting with the detection pipeline.
- **REST API Ready**: Easily adaptable for deployment as a REST API.
- **Scalable Model**: Suitable for integration into larger medical imaging platforms.

## Setup and Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/bhuvannv13/Brain_Tumour_detection_api.git
   cd Brain_Tumour_detection_api
   ```

2. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Ensure you have Jupyter Notebook installed for running the interactive notebook:
   ```bash
   pip install notebook
   ```

4. (Optional) Set up a virtual environment to isolate dependencies:
   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: .\env\Scripts\activate
   ```

## Usage

1. Open the Jupyter Notebook:
   ```bash
   jupyter notebook "Brain Tumour Detection.ipynb"
   ```

2. Follow the steps in the notebook to load the model, preprocess data, and make predictions.

3. To adapt the project for API deployment, consider using Flask or FastAPI. Refer to the code structure and ensure the model file is saved for reuse.

## Model and Methodology

- **Data Preprocessing**: The input MRI scans are preprocessed for model compatibility, including resizing, normalization, and augmentation.
- **Model Architecture**: The project employs a CNN architecture optimized for medical image analysis.
- **Evaluation Metrics**: The model's performance is evaluated using accuracy, precision, recall, and F1-score.
- **Training**: Ensure proper training data with tumour and non-tumour classifications for optimal results.

## Results

- Achieves high accuracy in detecting tumours from MRI scans.
- Visualizes predictions with overlays to assist in understanding model decisions.

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes and push to the branch.
   ```bash
   git push origin feature-name
   ```
4. Create a pull request describing your changes.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

For questions or feedback, please reach out via the repository's Issues section.


