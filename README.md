# Flask Prediction App

This is a simple Flask-based web application that loads a pre-trained machine learning model and uses it to make predictions based on user input. The app takes three numerical inputs, performs prediction with the model, and displays the prediction result categorized into different levels (e.g., "No", "Low", "Moderate", "High", "Very High").

## Features

- **Home Page**: The landing page of the app.
- **Prediction Page**: Accepts numerical input, applies the machine learning model, and displays a categorized prediction.
- **About Project Page**: Information about the project and its objectives.
- **Error Page**: Displays an error page in case of issues.

## Setup

### 1. Clone the repository:

```bash
git clone https://github.com/your-username/flask-prediction-app.git
```

### 2. Navigate to the project directory:

```bash
cd flask-prediction-app
```

### 3. Install the required dependencies:

You can install the necessary dependencies using `pip` by creating a `requirements.txt` file with the following content:

```
Flask==2.2.3
numpy==1.21.0
```

Run the following command to install the dependencies:

```bash
pip install -r requirements.txt
```

### 4. Place your model file (`model.pkl`) in the project directory:

Ensure that the pre-trained model file (`model.pkl`) is placed in the same directory as the app.

### 5. Run the application:

```bash
python app.py
```

The app will start running locally. Open a web browser and navigate to [http://127.0.0.1:5000](http://127.0.0.1:5000) to view the application.

## App Overview

### Routes

- `/`: Home route that greets the user.
- `/home`: Another route to the homepage (`homepage.html`).
- `/error`: Displays an error page (`error.html`).
- `/aboutproject`: Displays information about the project (`aboutproject.html`).
- `/prediction`: Handles the user input for prediction. It processes the input data and shows the prediction result.

### Prediction Logic

The app uses a machine learning model (`model.pkl`) to make predictions based on three numerical inputs. The prediction is categorized into different levels:

- **No**: The prediction value is less than 4.
- **Low**: The prediction value is between 4 and 6.
- **Moderate**: The prediction value is between 6 and 8.
- **High**: The prediction value is between 8 and 9.
- **Very High**: The prediction value is greater than 9.

If the prediction is not in any of these ranges, it will return an undefined result.

### Example

The user inputs three numerical values, and based on the model's prediction, the output is displayed with a category (e.g., Low, High).

## License

This project is open-source and available under the MIT License. See the [LICENSE](LICENSE) file for more information.

## Acknowledgments

- **Flask**: For the web framework used to build the app.
- **NumPy**: For handling numerical operations.
- **Pickle**: For loading the pre-trained machine learning model.

For any further questions or suggestions, please feel free to raise an issue in the repository.
```

