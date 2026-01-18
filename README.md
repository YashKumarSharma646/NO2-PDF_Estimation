# NO2 PDF Estimation using Non-Linear Transformation

This project estimates the probability density function (PDF) of NO2 air quality data using a roll-number-based non-linear transformation.

## Dataset
- Source: India Air Quality Dataset (Kaggle)
- Feature used: NO2

## Non-Linear Transformation
The input variable x is transformed as:

z = x + a_r sin(b_r x)

where:
- a_r = 0.05 × (r mod 7)
- b_r = 0.3 × (r mod 5 + 1)

## Results

### Histogram of Transformed Variable
![Histogram](outputs/histogram_z.png)

### Estimated Probability Density Function
![PDF Fit](outputs/pdf_fit.png)

## Files in this Repository
- analysis.ipynb : Jupyter notebook containing implementation
- data/ : Dataset files
- outputs/ : Generated plots
- requirements.txt : Required Python libraries

## Tools Used
- Python
- NumPy
- Pandas
- Matplotlib
