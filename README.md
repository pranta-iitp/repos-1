# Fashion MNIST Split Dataset

This repository contains the Fashion MNIST dataset divided into seven equal parts for efficient handling and experimentation in machine learning projects.

## About the Dataset

Fashion MNIST is a widely used benchmark dataset of 70,000 grayscale images (28x28 pixels) representing 10 categories of fashion items:
- T-shirt/top
- Trouser
- Pullover
- Dress
- Coat
- Sandal
- Shirt
- Sneaker
- Bag
- Ankle boot

## Repository Structure

- The dataset is split into seven CSV files: `part_1.csv` to `part_7.csv`.
- Each file contains 10,000 samples.
- All files are available in the `master` branch.

## How to Use

1. **Download the required CSV files from this repository.**
2. **Load a part in Python using pandas:**
```
import pandas as pd
df = pd.read_csv('part_1.csv') # Replace with the desired part
```
3. **To combine all parts into a single DataFrame:**
```
import pandas as pd
parts = [pd.read_csv(f'part_{i}.csv') for i in range(1, 8)]
full_df = pd.concat(parts, ignore_index=True)
```
## Intended Use

- For training, testing, and experimenting with machine learning models in Python and PyTorch.
- Designed for use in environments like Google Colab, especially where file size limits apply.

## Notes

- The dataset is split to facilitate easier download and processing.
- All split files are available in the `master` branch.

