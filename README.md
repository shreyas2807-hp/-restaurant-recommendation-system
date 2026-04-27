# **Restaurant Recommendation System**
---

## **Project Description**
- This project focuses on developing a smart restaurant recommendation system that delivers personalized suggestions based on user preferences, budget, dietary restrictions, and current location.
- A hybrid recommendation model combining **collaborative filtering** and **content-based filtering** techniques is implemented to provide accurate and relevant results.
- The system adapts dynamically based on user inputs and geolocation data, enhancing the user's decision-making process when exploring dining options.

## **Screenshots**

### Home Page:
<p align="center">
<img src="https://drive.google.com/uc?export=view&id=10fcQJ3leJHaBbSt4LqKCr7bO7v3jIE3Y" width="800" alt="Image1">

</p>

### Input Page:
<p align="center">
<img src="https://drive.google.com/uc?export=view&id=1K5ugAoJ4C9wukRHvOFfWtfHl3Jp2mm29" width="800" alt="Image2">

</p>

### Recommendation Output:
<p align="center">
 <img src="https://drive.google.com/uc?export=view&id=1iF3VR3lRywqaR1YVP0oDlihbbo_OjJ16" width="800" alt="Image3">

</p>

## **Installation and Setup**

### Using Conda (Recommended)
```bash
# Create a new conda environment
conda create -n restaurant_recommender python=3.10

# Activate the environment
conda activate restaurant_recommender

# Clone the repository
git clone https://github.com/raju2703/ADS_Restaurant_Recommendation_System.git
cd ADS_Restaurant_Recommendation_System/Flask

# Install dependencies
pip install -r requirements.txt
```
### Using Python venv
```bash
# Create a virtual environment
python -m venv venv

# Activate the environment
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt
```

### Running the Application
```bash
# Navigate to the Flask directory
cd Flask

# Run the Flask web application
python app.py

# Visit http://localhost:5000 to access the app
```
### Project Structure:

```bash
Restaurant-Recommendation-System/
├── Documentation...
├── Flask/
│   ├── __pycache__/                # Compiled Python cache files
│   ├── static/                     # Static assets (Images)
│   ├── templates/                  # HTML templates for the frontend
│   ├── app.py                     # Flask application entry point
│   ├── Final_Development_Phase.ipynb  # Flask dev notebook
│   ├── requirements.txt            # Python dependencies
│   └── restaurant.csv             # Restaurant dataset
├── Model/
    └── Final_Development_Phase.ipynb  # Model training and evaluation notebook
```

## **Technologies Used**
- **Python 3.10** – Core programming language
- **Flask** – Lightweight web framework to build the backend API
- **Scikit-learn** – For building and evaluating machine learning models
- **Surprise** – Specialized library for collaborative filtering (e.g., SVD)
- **Pandas / NumPy** – For data manipulation and preprocessing
- **NLTK** – For natural language processing and cleaning review text
- **Matplotlib / Seaborn / Plotly** – For data visualization and EDA
- **HTML / CSS / JavaScript** – For designing the frontend interface

---

## **Model Architecture**
This project uses a **Hybrid Recommendation Model** combining the strengths of:

### 🔹 Content-Based Filtering
- Analyzes restaurant attributes like cuisine type, average cost, rating, and delivery option.
- Matches these with user-stated preferences to recommend relevant restaurants.

### 🔹 Collaborative Filtering (SVD)
- Uses historical user rating data to find similar users and suggest restaurants based on collective behavior.
- Implemented using the `Surprise` library's Singular Value Decomposition (SVD) algorithm.

### 🔹 Hybrid Approach
- Merges both filtering strategies to solve the cold-start and sparsity problems.
- Balances personalization with discovery of new or less popular options.

## **Dataset**
The dataset is sourced from **Kaggle** and titled:

> [Zomato Bangalore Restaurants Dataset by Himanshu Poddar](https://www.kaggle.com/datasets/himanshupoddar/zomato-bangalore-restaurants)

## **Conclusion**
This project successfully demonstrates how **machine learning and recommendation systems** can simplify dining decisions by tailoring restaurant suggestions to user preferences and behavior. It offers a powerful and adaptive solution for users in both familiar and unfamiliar areas. The hybrid model ensures balance between personalized results and discovery of new options. This project lays the foundation for more advanced, real-time, and location-aware food recommendation engines.



