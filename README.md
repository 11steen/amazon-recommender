# Amazon Product Recommendation App

A Streamlit-based web application that recommends the top 5 personalized products to users based on their past rating behavior and similar users’ preferences.

This project uses a user-based collaborative filtering approach trained on Amazon product reviews to generate tailored product recommendations.

---

## Dataset

**amazon_reviews.csv** – contains user IDs, product IDs, and ratings.

- 500K+ product ratings  
- Used to build user-item interaction matrix  
- Source: [Kaggle – Amazon Reviews Dataset](#)

---

## Features

- Recommends top 5 products per user based on rating behavior
- Collaborative filtering using user similarity
- Streamlit interface with dropdown for user selection
- Clean layout with real-time product suggestions

---

## Tech Stack

- **Language**: Python  
- **Libraries**: Pandas, NumPy, Scikit-learn  
- **Web App**: Streamlit  
- **Structure**: Modular Python scripts (`/src`) + Jupyter notebook for training

---

## Project Structure
📁 src/
├── amazon_recommendation_app.py # Streamlit app
├── training.py # Recommendation logic
├── utils.py # Helper functions
├── EDA.py # Optional: Exploratory Data Analysis
📄 Amazon product ratings prediction.ipynb
📄 amazon_reviews.csv


---

## Installation & Usage

```bash
# 1. Clone the repository
git clone https://github.com/yourusername/amazon-recommendation-app.git
cd amazon-recommendation-app

# 2. Install dependencies
pip install streamlit pandas numpy scikit-learn

# 3. Run the app
streamlit run src/amazon_recommendation_app.py

Future Improvements
Add product metadata (title, images)

Enhance recommendation algorithm (e.g., SVD, hybrid methods)

Add login/user session support




