# Emergency Health Alert System Using Machine Learning and Deep Learning

An AI-assisted health screening web application designed to explore potential health risks using Machine Learning and Deep Learning techniques.

**Live Demo:** https://emergency-health-alert-system.onrender.com/

**GitHub Repository:** https://github.com/Hariprasad2812/-Emergency-Health-Alert-System

## Project Overview

The Emergency Health Alert System is a web application that brings together predictive models for three health-related screening tasks:

- **Heart Disease Prediction:** Estimates potential heart disease risk from clinical input features using a Random Forest classification model.
- **Kidney Disease Prediction:** Supports chronic kidney disease risk screening using relevant clinical and laboratory inputs.
- **Skin Lesion Analysis:** Uses a deep learning model based on MobileNetV2 to analyze uploaded skin lesion images.

The application provides a web interface for users to access the available features.

## Features

- Heart disease risk prediction.
- Kidney disease risk screening.
- AI-assisted skin lesion image analysis.
- Web interface with home, methodology, login, and registration pages.
- Flask-based backend.
- Machine Learning and Deep Learning model integration.
- Online deployment using Render.

## Technologies Used

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| Flask | Web application framework |
| Scikit-learn | Machine Learning |
| TensorFlow / Keras | Deep Learning |
| Random Forest | Heart disease classification |
| MobileNetV2 | Skin lesion image analysis |
| HTML and CSS | Web interface |
| Pandas and NumPy | Data processing |
| Gunicorn | Production WSGI server |
| Git and GitHub | Version control and source code hosting |
| Render | Web application deployment |

## Project Structure

```text
Emergency-Health-Alert-System/
├── app.py
├── Train.py
├── requirements.txt
├── runtime.txt
├── .python-version
├── .gitignore
├── README.md
├── models/
├── templates/
├── static/
├── Split_smol/
├── heart.csv
└── kidney_disease.csv
```

The `models/` directory contains the trained model files. The `templates/` directory contains HTML templates, and `static/` contains frontend assets such as CSS.

## Run the Project Locally

### 1. Clone the repository

```bash
git clone https://github.com/Hariprasad2812/-Emergency-Health-Alert-System.git
cd -Emergency-Health-Alert-System
```

### 2. Create a virtual environment

Windows PowerShell:

```powershell
python -m venv venv
.\venv\Scripts\Activate.ps1
```

### 3. Install dependencies

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### 4. Start the application

```bash
python app.py
```

Open the following address in your browser:

http://127.0.0.1:5000/

Keep the terminal running while using the local application.

**Note:** Use a Python version compatible with the dependencies listed in `requirements.txt`. If model loading fails, check the installed TensorFlow, Keras, NumPy, and scikit-learn versions.

## Deploy on Render

The application is deployed using Render.

1. Push the project to GitHub.
2. Sign in to [Render](https://dashboard.render.com/).
3. Create a Web Service and connect this repository.
4. Set the build command to:

   ```bash
   pip install -r requirements.txt
   ```

5. Set the start command to:

   ```bash
   gunicorn app:app
   ```

6. Select the appropriate Python runtime.
7. Deploy the service and review the build and runtime logs.

The repository root should contain `app.py` and `requirements.txt` for these commands to work without additional directory configuration.

Live application: https://emergency-health-alert-system.onrender.com/

## How It Works

1. The user opens the web application.
2. The user selects an available health screening feature.
3. The application collects the required clinical inputs or image.
4. The corresponding trained model processes the input.
5. The application displays the model's prediction or assessment.

Actual behavior depends on the implementation and the available model files.

## Future Improvements

- Improve prediction validation and error handling.
- Add comprehensive model evaluation metrics.
- Improve accessibility and mobile responsiveness.
- Add secure authentication and persistent user storage where required.
- Improve model monitoring and deployment reliability.
- Document datasets, model limitations, and reproducibility.

## Disclaimer

This project is intended for educational, research, and preliminary screening purposes only. Its predictions are not medical diagnoses and should not be used as the sole basis for treatment or emergency decisions.

Consult a qualified healthcare professional for medical advice. Seek emergency medical care when necessary.

## Author

**Hariprasad2812**

GitHub: https://github.com/Hariprasad2812

## License

No license has been specified for this repository yet. Add a license file if you intend to grant others permission to use, modify, or distribute the project.
