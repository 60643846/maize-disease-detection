# Maize Disease Detection Using MobileNetV2

Adapting MobileNetV2 for noisy plant images in greenhouse environments.

## Overview
This project tests whether models trained on clean laboratory images can detect plant diseases from noisy smartphone photos taken in real greenhouses. Focus: **Maize Streak Virus (MSV)** and **Maize Leaf Blight (MLB)**.

## Results
- Clean images: **98.91%** accuracy
- Noisy images (original): **54.33%** accuracy  
- Noisy images (preprocessed): **51%** accuracy
- Noisy images (fine-tuned): **78.33%** accuracy



## Installation
```bash
pip install -r requirements.txt
```

## Running the Project
Double-click `start_project.bat` or run:
```bash
jupyter notebook
```

## Project Structure
```
data/raw/          Raw images (download separately)
notebooks/         Main implementation notebook
results/           Confusion matrices and figures
models/            Saved model files
```

## Key Finding
Fine-tuning on noisy images improved accuracy by 24 percentage points, while preprocessing made performance worse. This shows models must be adapted to target conditions, not just applied with cleaned-up inputs.
