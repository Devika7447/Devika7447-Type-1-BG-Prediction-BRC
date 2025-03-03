# Type-1-BG-Prediction-BRC

Predicting blood glucose levels in Type 1 diabetes (T1D) is of utmost importance due to its direct impact on patient safety, long-term health, and overall quality of life. Maintaining blood sugar within a safe range is critical for preventing life-threatening complications and improving daily diabetes management. One of the most immediate concerns in T1D is preventing hypoglycemia (low blood sugar) and hyperglycemia (high blood sugar). Predicting glucose levels enables timely interventions, such as consuming carbohydrates to prevent a sugar crash or adjusting insulin doses to avoid dangerous spikes.

Accurate blood glucose prediction in Type 1 diabetes is essential for preventing long-term complications such as nerve damage, kidney failure, heart disease, and blindness by maintaining better glycemic control.

Since glucose levels are influenced by multiple factors like diet, stress, and exercise, predictive models help reduce the mental and physical burden on patients and caregivers by providing automated assistance.

## 📌BIDIRECTIONAL RESERVOIR COMPUTING

Reservoir Computing (RC) is a paradigm for training recurrent neural networks (RNNs) where the recurrent part (the "reservoir") is fixed and only the readout layer is trained. The reservoir projects the input data into a higher-dimensional space, and Ridge Regression maps the reservoir states to the target variable. Bidirectional Reservoir Computing combines two reservoirs: Forward Reservoir and Backward Reservoir

**How It Works?**

Input Transformation: Sequential data (glucose readings) is fed into the forward and backward reservoirs.

Reservoir Dynamics: The reservoirs transform the input data into a high-dimensional state space using fixed recurrent connections. The forward reservoir captures the influence of past data, while the backward reservoir captures future dependencies.

Readout Learning: A trainable readout layer combines the outputs from both reservoirs to predict the target 

Prediction: After training, the model predicts new sequences using the readout layer.

## 🚀 Features of the BRC Model

- **Biologically Relevant Constraints (BRC)**: Integrates physiological constraints to enhance blood glucose prediction accuracy.
- **Advanced Data Preprocessing**: Combines multiple datasets, handles missing values, and applies feature engineering techniques.
- **Deep Learning with DCNN**: Utilizes a Deep Convolutional Neural Network (DCNN) for time-series blood glucose prediction.
- **Feature Selection Optimization**: Identifies the most significant features, improving model interpretability and accuracy.
- **Custom Hyperparameter Tuning**: Supports adjustable batch size, epochs, and learning rate for optimized performance.
- **Multi-Source Data Integration**: Merges glucose readings, insulin intake, carbohydrate consumption, and activity levels for holistic prediction.
- **Performance Metrics**: Evaluates model performance using Mean Absolute Error (MAE), Root Mean Square Error (RMSE), and other key metrics.


## 🔧 Requirements

To run this project, ensure you have the following dependencies installed:  

### 📌 Required Libraries  
- Python 3.8+  
- TensorFlow 2.5+  
- NumPy  
- Pandas  
- Scikit-learn  
- Matplotlib  
- Seaborn  
- Keras  
- SciPy  


**📊About The Dataset : HUPA-UCM DIABETES DATASET**

The dataset consists of multiple CSV files, each named with an identifier (e.g., "HUPA0001P.csv" to "HUPA0028P.csv"). These represent individual patient records or data segments.

**Summary of the Data:**

- Time-based dataset: Each row represents a timestamped health measurement.
- Glucose levels: Monitors blood glucose over time.
- Physical activity: Tracks calories burned and steps taken.
- Heart rate: Records fluctuations in heart rate.
- Insulin management: Captures basal insulin rate and bolus insulin delivery.
- Dietary intake: Logs carbohydrate consumption.

## ⚙ Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Devika7447/Type-1-Diabetes-BG-Prediction-BRC.git

## 🙌 Acknowledgments

- This project is inspired by ongoing research in **blood glucose prediction** for Type-1 Diabetes management.
- Special thanks to **researchers and healthcare professionals** working to improve diabetes prediction and treatment.
- Gratitude to the **open-source community** for providing essential libraries like TensorFlow, Pandas, and Scikit-learn, which made this project possible.
- Thanks to all contributors who helped refine the model and enhance its performance.




