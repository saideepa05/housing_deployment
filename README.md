# California Housing Price Prediction

This project is a complete end-to-end Machine Learning deployment pipeline. It utilizes a Linear Regression model to predict housing prices in California based on several features.

## 🚀 Work History & Achievements

1.  **Model Regeneration:** Resolved `scikit-learn` version mismatch warnings by retraining the model and scaler using the local environment's version.
2.  **Web Application:** Developed a Flask-based web interface with a professional dark-themed UI.
3.  **API Development:** Implemented a robust `/predict` endpoint that handles numeric data validation and explicit feature mapping.
4.  **Dockerization:** Created a `Dockerfile` for containerized deployment.
5.  **CI/CD Pipeline:** Configured GitHub Actions (`main.yaml`) for automatic deployment to Heroku upon code push.
6.  **Environment Stability:** Integrated Heroku CLI installation in the CI/CD workflow to fix common "spawn heroku ENOENT" errors.

## 🛠️ Tech Stack
- **Framework:** Flask
- **Machine Learning:** Scikit-Learn, Pandas, Numpy
- **Styling:** Vanilla CSS (Custom dark theme)
- **Deployment:** Docker, Heroku
- **Automation:** GitHub Actions

## 💻 Local Setup

**1. Create the environment:**
```powershell
conda create -p venv python==3.7 -y
```

**2. Activate the environment:**
```powershell
conda activate ./venv
```

**3. Install dependencies:**
```powershell
pip install -r requirements.txt
```

**4. Run the app:**
```powershell
python app.py
```

## 🐳 Docker Usage

To build and run the application locally using Docker:

```bash
docker build -t housing-app .
docker run -p 5000:5000 housing-app
```

## ☁️ Deployment (Heroku)

This project is set up for automatic deployment via GitHub Actions.
1. Add your `HEROKU_EMAIL`, `HEROKU_API_KEY`, and `HEROKU_APP_NAME` to GitHub Secrets.
2. Push to the `main` branch.
3. The workflow in `.github/workflows/main.yaml` will handle the building and releasing of your Docker container.
