# Customer Churn Prediction using Artificial Neural Networks 🎯

This project implements a machine learning solution to predict customer churn in a banking context using Artificial Neural Networks (ANN). The model analyzes various customer attributes to predict whether a customer is likely to leave the bank.

## 🔴 Live Demo
Check out the live application: [Bank Customer Churn Predictor](https://churn-prediction-mkc6xwmyt27rlps7noqebq.streamlit.app/)


![Bank Churn](https://imgs.search.brave.com/3wuPh_SHH-BUiLRKD_XBSTyAO5OLQqaXHWaONQGWb7M/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly9tZWRp/YS5saWNkbi5jb20v/ZG1zL2ltYWdlL0Q0/RDEyQVFIZFY1enRi/ck12UGcvYXJ0aWNs/ZS1jb3Zlcl9pbWFn/ZS1zaHJpbmtfNjAw/XzIwMDAvMC8xNjky/NjQxNTEzMTI4P2U9/MjE0NzQ4MzY0NyZ2/PWJldGEmdD1QN2kz/NlZGR1M1WUJtaHNW/MmtJTG9Cc2hhYS03/U1hZbVdqOEZuUDVR/SjVN)

## 📊 Project Overview

The system predicts customer churn based on features including:
- Credit Score
- Gender
- Age
- Tenure
- Balance
- Number of Products
- Credit Card Status
- Activity Status
- Estimated Salary
- Geography (France, Germany, Spain)

## 🗂️ Project Structure

```
├── data/               # Data files directory
├── logs/              # Training logs
├── venv/              # Python virtual environment
├── app.py             # Streamlit application file
├── experiments.ipynb  # Experimentation notebook
├── prediction.ipynb   # Prediction examples
├── model.h5           # Trained neural network model
├── sc.pkl            # Standard scaler object
├── ohe_geo.pkl       # One-hot encoder for geography
├── label_encoder_gender.pkl  # Label encoder for gender
└── requirements.txt   # Project dependencies
```

## 🚀 Getting Started

### Prerequisites

- Python 3.12
- pip package manager

### Installation

1. Clone the repository:
```bash
git clone https://github.com/Priyanshu1303d/churn-prediction.git
cd churn-prediction
```

2. Create and activate virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install required packages:
```bash
pip install -r requirements.txt
```

## 💻 Usage

### Running Locally with Streamlit

Run the Streamlit application:
```bash
streamlit run app.py
```

The application will open in your default web browser.

### Deploying to Streamlit Cloud

1. Push your code to GitHub
2. Visit [Streamlit Cloud](https://streamlit.io/cloud)
3. Create a new app and connect it to your GitHub repository
4. Select app.py as the main file
5. Deploy!


## 🔄 Model Pipeline

1. **Data Preprocessing**:
   - Gender encoding using LabelEncoder
   - Geography encoding using OneHotEncoder
   - Feature scaling using StandardScaler

2. **Model Architecture**:
   - Input Layer: Features dimension
   - Hidden Layers: Dense layers with ReLU activation
   - Output Layer: Single neuron with sigmoid activation

## 📦 Dependencies

Main dependencies include:
- TensorFlow
- Keras
- scikit-learn
- pandas
- numpy
- streamlit

See `requirements.txt` for complete list.

## 🛠️ Development

To experiment with the model:
1. Open `experiments.ipynb` for model training and evaluation
2. Use `prediction.ipynb` for testing predictions
3. Modify `app.py` for Streamlit interface changes

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 📧 Contact

Project Link: [https://github.com/Priyanshu1303d/churn-prediction](https://github.com/Priyanshu1303d/churn-prediction)

Built by Priyanshu
