# Spotify Hybrid Recommender System

A powerful music recommendation system that combines content-based and collaborative filtering techniques to provide personalized song suggestions from the Spotify music catalog.

## 🎯 Features

- **Hybrid Recommendation Engine**: Combines content-based and collaborative filtering for more accurate recommendations
- **Multiple Recommendation Modes**:
  - Content-based filtering
  - Collaborative filtering
  - Hybrid approach (combination of both)
- **Interactive Web Interface**: Built with Streamlit for easy interaction
- **Data Processing Pipeline**: Includes data cleaning and transformation steps
- **Scalable Architecture**: Designed to handle large music datasets

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- pip (Python package manager)
- DVC (Data Version Control) - for data versioning

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/VHemanth45/Spotify-Hybrid-Recommender-System.git
   cd Spotify-Hybrid-Recommender-System
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up DVC (if you want to track data versioning):
   ```bash
   pip install dvc
   dvc pull  # To download the data files
   ```

## 🎵 Dataset

The system uses the following datasets:
- `Music Info.csv`: Contains detailed information about songs
- `User Listening History.csv`: Contains user listening data for collaborative filtering

## 🛠️ Project Structure

```
├── data/                    # Data files
│   ├── cleaned_data.csv      # Processed and cleaned data
│   ├── collab_filtered_data.csv  # Pre-filtered data for collaborative filtering
│   └── ...
├── notebooks/               # Jupyter notebooks for EDA
│   └── EDA_Spotify_Dataset.ipynb
├── app.py                   # Main Streamlit application
├── content_based_filtering.py  # Content-based recommendation logic
├── collaborative_filtering.py  # Collaborative filtering implementation
├── hybrid_recommendations.py   # Hybrid recommendation system
├── data_cleaning.py         # Data preprocessing scripts
├── transform_filtered_data.py  # Data transformation utilities
├── requirements.txt         # Python dependencies
└── README.md               # This file
```

## 🎛️ Usage

1. Start the Streamlit application:
   ```bash
   streamlit run app.py
   ```

2. Open your web browser and navigate to the provided local URL (typically http://localhost:8501)

3. In the web interface:
   - Enter a song name and artist
   - Select the number of recommendations you want
   - Choose the recommendation type (Content-based, Collaborative, or Hybrid)
   - Click "Get Recommendations"

## 🤖 Recommendation Methods

### 1. Content-based Filtering
Recommends songs similar to a given song based on audio features like danceability, energy, tempo, etc.

### 2. Collaborative Filtering
Recommends songs based on user listening patterns and preferences from similar users.

### 3. Hybrid Approach
Combines both content-based and collaborative filtering to provide more accurate and diverse recommendations.

## 📊 Data Processing Pipeline

1. **Data Cleaning**:
   - Handling missing values
   - Removing duplicates
   - Normalizing text data
   - Feature engineering

2. **Feature Engineering**:
   - Extracting audio features
   - Creating user-item interaction matrices
   - Dimensionality reduction

3. **Model Training**:
   - Training content-based models
   - Building collaborative filtering models
   - Implementing hybrid recommendation logic

## 📦 Dependencies

Key Python packages used in this project:
- Streamlit - Web application framework
- NumPy & Pandas - Data manipulation
- Scikit-learn - Machine learning algorithms
- SciPy - Scientific computing
- DVC - Data version control


## 📬 Contact

VHemanth45 - [GitHub Profile](https://github.com/VHemanth45)

---

Built with ❤️ for music lovers and data science enthusiasts!