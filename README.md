📦 Amazon Electronics Recommendation Engine
A machine learning-powered recommendation system built using real-world Amazon Electronics data. It predicts product preferences based on historical user ratings and suggests similar items using collaborative filtering (SVD).

🚀 Features
📊 Uses collaborative filtering (SVD) for personalized recommendations

🧠 Predicts user preferences based on past interactions

📈 Scalable for large datasets with sparse matrices

💬 Provides product-based filtering using product names (not raw IDs)

🖥️ Clean and intuitive Streamlit web interface

🌄 Beautiful UI with animated background and card-style recommendations

📂 Dataset
Source: Amazon Electronics product reviews

Key Columns:

userName: Reviewer name

item_id: Unique product ID

rating: Rating given by the user

reviewText: Detailed review text

itemName, brand, category, etc.

Note: Large metadata files are currently replaced with mock product titles to ensure smooth app performance and cleaner display.

🧠 Approach
Data Preprocessing: Cleaned ratings and handled missing values

Matrix Factorization: Applied Truncated SVD to the user-item rating matrix

Top-N Recommendations: Finds top similar products based on learned latent features

Name Mapping: Replaces technical item IDs with real or mock product names for user-friendly recommendations

🖥️ Web App
Built using Streamlit, the app allows users to:

🔍 Select a product by name from a dropdown

📃 View top recommended products

🎨 Experience a visually appealing UI with slideshow background and card-styled results

⚙️ How to Run
bash
Copy code
# Clone the repository
git clone https://github.com/11steen/amazon-recommender.git
cd amazon-recommendation-engine

# Install dependencies
pip install -r requirements.txt

# Run the app
streamlit run app.py
🛠️ Tech Stack
Python, Pandas, NumPy

Scikit-learn (Truncated SVD)

Streamlit for interactive UI
