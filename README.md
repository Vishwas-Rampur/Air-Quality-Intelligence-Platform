# Air Quality Intelligence Platform

An AI-powered environmental monitoring platform that transforms coarse-resolution satellite NO₂ data into high-resolution air quality maps using machine learning.

## Project Overview

The Air Quality Intelligence Platform uses satellite-derived NO₂ observations and machine learning techniques to generate enhanced air-quality maps with improved spatial resolution.

The application provides an interactive dashboard where users can:

- Upload satellite NO₂ datasets
- Process and clean environmental data
- Generate downscaled air-quality maps
- Visualize pollution patterns
- Evaluate model performance
- Download prediction results

This project is designed for environmental researchers, students, policy makers, and organizations interested in air-quality monitoring.

---

## Features

- Satellite NO₂ data analysis
- Machine Learning based downscaling
- Interactive Plotly visualizations
- GeoTIFF support
- Ground station data integration
- Performance metrics (RMSE, R², MSE)
- Streamlit web dashboard
- Database-backed storage

---

## Technology Stack

### Frontend
- Streamlit

### Data Processing
- NumPy
- Pandas

### Visualization
- Plotly

### Machine Learning
- Scikit-learn
- Random Forest Regressor

### Geospatial Processing
- Rasterio

### Database
- SQLite
- SQLAlchemy

### Python Version
- Python 3.11+

---

## Project Structure

```text
Air-Quality-Intelligence-Platform/
│
├── main.py
├── model.py
├── utils.py
├── database.py
├── styles.css
├── pyproject.toml
├── README.md
│
└── no2_data.db (generated automatically)
```

---

## Machine Learning Workflow

```text
Satellite NO₂ Data
        │
        ▼
Data Cleaning
        │
        ▼
Feature Engineering
        │
        ▼
Random Forest Model
        │
        ▼
High Resolution Prediction
        │
        ▼
Interactive Visualization
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/Vishwas-Rampur/Air-Quality-Intelligence-Platform.git
```

Navigate to the project:

```bash
cd Air-Quality-Intelligence-Platform
```

Create a virtual environment:

```bash
py -m venv .venv
```

Activate the environment:

```bash
.venv\Scripts\activate
```

Install dependencies:

```bash
pip install numpy pandas plotly psycopg2-binary python-dotenv rasterio scikit-learn sqlalchemy streamlit
```

Run the application:

```bash
python -m streamlit run main.py
```

Open:

```text
http://localhost:8501
```

---

## Usage

### Step 1
Upload a satellite NO₂ GeoTIFF file.

### Step 2
(Optional) Upload ground station measurements in CSV format.

### Step 3
Run the machine learning downscaling process.

### Step 4
Visualize the generated high-resolution pollution map.

### Step 5
Review model performance metrics and download results.

---

## Supported Data Sources

### Satellite Data

- Sentinel-5P (TROPOMI)
- NASA EarthData
- OMI Aura

### Ground Measurements

- CPCB Air Quality Stations
- Local monitoring stations

---

## Performance Metrics

The platform evaluates prediction quality using:

- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

---

## Future Improvements

- XGBoost integration
- Deep Learning models
- Real-time satellite ingestion
- Weather data integration
- Interactive GIS maps
- Automated reporting
- Cloud deployment

---

## Author

**Vishwas Rampur**

GitHub:
https://github.com/Vishwas-Rampur

---

## License

MIT License