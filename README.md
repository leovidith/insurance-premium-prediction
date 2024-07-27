# Insurance Charges Prediction

This project demonstrates a regression model built using TensorFlow to predict insurance charges based on various features. The dataset used is the "insurance" dataset from a public repository.

## Features

- **Data Preprocessing**: Normalization of numerical features and one-hot encoding of categorical features.
- **Model Architecture**: A neural network with dropout layers for regularization.
- **Training & Evaluation**: Model training with early stopping and evaluation on test data.
- **Visualization**: Plotting training and validation loss over epochs.

## Requirements

- Python 3.x
- TensorFlow
- Pandas
- NumPy
- Matplotlib
- scikit-learn

## Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/yourusername/Insurance-Charges-Prediction.git
    ```

2. **Navigate to the project directory:**

    ```bash
    cd Insurance-Charges-Prediction
    ```

3. **Create and activate a virtual environment (optional but recommended):**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

4. **Install the required packages:**

    ```bash
    pip install tensorflow pandas numpy matplotlib scikit-learn
    ```

## Usage

1. **Run the script:**

    Execute the following command to preprocess the data, build and train the model, and visualize the results:

    ```bash
    python train_model.py
    ```

2. **Script Details:**

    - **Data Loading**: Reads the insurance dataset from a public URL.
    - **Preprocessing**: Normalizes numerical features, one-hot encodes categorical features.
    - **Model Building**: Defines and compiles a neural network model.
    - **Training**: Trains the model and uses early stopping to avoid overfitting.
    - **Evaluation**: Evaluates the model on test data.
    - **Visualization**: Plots training and validation loss.


### Output

The script will output the final evaluation metrics of the model and display a plot of the training and validation loss over epochs.
