Certainly! Here is the full updated `README.md` including your original content plus the **Image Preprocessing** section inserted between **Usage** and **Model and Methodology**:

````markdown
# Brain Tumour Classification API

This repository provides a Python-based API for detecting brain tumours from medical images. The solution uses deep learning models to identify tumours and includes an interactive notebook for running the classification pipeline.

## Table of Contents
- Overview
- Features
- Setup and Installation
- Usage
- Image Preprocessing (Gaussian, Median, Negative Filtering)
- Model and Methodology
- Results
- Contributing
- License

---

## Overview

Brain tumours are serious medical conditions requiring early detection  and classififcation for effective treatment. This project provides an automated approach to classifying  brain tumours from medical imaging data using a convolutional neural network (CNN)-based classifier. The API is implemented in Python and uses Jupyter Notebook for demonstration.

---

## Features

- **Deep Learning-based Classification:** Utilizes CNNs for identifying  tumour types in MRI scans.  
- **Interactive Notebook:** Includes a notebook for experimenting with the detection pipeline.  
- **REST API Ready:** Easily adaptable for deployment in a Hudding face.  
- **Scalable Model:** Suitable for integration into larger medical imaging platforms.

---

## Setup and Installation

Clone the repository:

```bash
git clone https://github.com/bhuvannv13/Brain_Tumour_classification_api.git
cd Brain_Tumour_classification_api
````

Install the required Python packages:

```bash
pip install -r requirements.txt
```

Ensure you have Jupyter Notebook installed for running the interactive notebook:

```bash
pip install notebook
```

(Optional) Set up a virtual environment to isolate dependencies:

```bash
python -m venv env
source env/bin/activate  # On Windows: .\env\Scripts\activate
```

---

## Usage

Open the Jupyter Notebook:

```bash
jupyter notebook "Brain Tumour Detection.ipynb"
```

Follow the steps in the notebook to load the model, preprocess data, and make predictions.

To adapt the project for API deployment, consider using Hugging face. Refer to the code structure and ensure the model file is saved for reuse.

---

## Image Preprocessing (Gaussian, Median, Negative Filtering)

This repository also contains Python scripts for preprocessing MRI brain tumour images using various filters including **Gaussian Blur**, **Median Filter**, and **Negative Filter**. The preprocessing is done class-wise on the **Glioma**, **Meningioma**, and **Pituitary** tumour datasets, divided into `Training` and `Testing` folders.

### Directory Structure

```
BrainTumor/
├── Training/
│   ├── filter/
│   │   ├── glioma_tumor/
│   │   ├── meningioma_tumor/
│   │   └── pituitary_tumor/
│   └── Negative/
│       ├── glioma_tumor/
│       ├── meningioma_tumor/
│       └── pituitary_tumor/
├── Testing/
│   ├── filter/
│   │   ├── glioma_tumor/
│   │   ├── meningioma_tumor/
│   │   └── pituitary_tumor/
│   └── Negative/
│       ├── glioma_tumor/
│       ├── meningioma_tumor/
│       └── pituitary_tumor/
```

### Tumor Classes

* `glioma_tumor`
* `meningioma_tumor`
* `pituitary_tumor`
*  `no_tumor`

### Requirements

You must install the following Python packages:

```bash
pip install opencv-python numpy
```

> If you encounter network errors like `getaddrinfo failed`, ensure your internet connection is active and that you're not behind a proxy or firewall blocking pip.

### Filters Applied

* **Gaussian Filter:** Removes noise and detail using a Gaussian kernel.
* **Median Filter:** Preserves edges while removing noise.
* **Negative Filter:** Inverts image colors for contrast enhancement.

### How to Use

1. Clone the repository:

```bash
git clone https://github.com/yourusername/brain-tumor-preprocessing.git
cd brain-tumor-preprocessing
```

2. Set the `img_dir` and `filtered_dir` paths in the scripts to your local dataset directories.

3. Run each script as required:

```bash
python gaussian_median_filter.py
python negative_filter.py
```

### Notes

* All scripts are written in Python using OpenCV.
* The datasets are assumed to be stored locally with class-wise subfolders.
* You can adapt these scripts for other filters or transformations.

### Author

**\[Your Name]**
\[Your Email] | \[LinkedIn] | [GitHub](https://github.com/yourusername)

### License

This project is open-source and available under the MIT License.

---

## Model and Methodology

* **Data Preprocessing:** The input MRI scans are preprocessed for model compatibility, including resizing, normalization, and augmentation.
* **Model Architecture:** The project employs a CNN architecture optimized for medical image analysis.
* **Evaluation Metrics:** The model's performance is evaluated using accuracy, precision, recall, and F1-score.
* **Training:** Ensure proper training data with tumour and non-tumour classifications for optimal results.

---

## Results

* Achieves high accuracy of 0.80 in classyfying tumours type from MRI scans.
* Visualizes predictions with overlays to assist in understanding model decisions.

---

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

---

## License

This project is licensed under the MIT License. See the LICENSE file for details.

```

---


```
