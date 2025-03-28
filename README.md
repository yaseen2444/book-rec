# Book Recommender System

## Project Overview
This is a machine learning-powered book recommendation application built using Streamlit, which suggests similar books based on a user's selected book.

## Author
- **Name:** Mohammad Yaseen
- **Email:** yaseenmohammadap37@gmail.com
- **Date:** January 19, 2025

## Live Demo
[Book Recommender App](https://book-rec-kueasys3vh3k64m3tyjeab.streamlit.app/)

## Features
- Interactive book selection dropdown
- Recommendation of 5 similar books
- Book cover images displayed with recommendations
- Uses k-Nearest Neighbors (KNN) algorithm for recommendations

## Technology Stack
- Python
- Streamlit
- Scikit-learn
- NumPy
- Pandas

## Project Structure
```
book-recommender/
│
├── data/
│   └── BX-Books.csv           # Original book dataset
│
├── artifacts/
│   ├── model.pkl               # Trained KNN model
│   ├── book_names.pkl          # List of book names
│   ├── final_rating.pkl        # Processed rating data
│   └── book_pivot.pkl          # Pivot table of book ratings
│
└── app.py                      # Streamlit application
```

## How It Works
1. The system uses a k-Nearest Neighbors algorithm to find similar books
2. It creates a sparse matrix from book ratings
3. When a book is selected, it finds the 5 most similar books based on user ratings

## Data Preprocessing
- Removed duplicate entries
- Created a pivot table of book ratings
- Converted data to a sparse matrix for efficient computation

## Installation
1. Clone the repository
2. Install dependencies:
   ```
   pip install streamlit numpy pandas scikit-learn
   ```
3. Run the application:
   ```
   streamlit run app.py
   ```

## Dependencies
- streamlit
- numpy
- pandas
- scikit-learn

## Recommendation Method
Uses collaborative filtering with k-Nearest Neighbors algorithm to suggest books based on:
- Similar user ratings
- Book characteristics
- Proximity in the feature space

## Limitations
- Recommendations based on available dataset
- Requires sufficient rating data for accurate suggestions

## Future Improvements
- Implement more advanced recommendation algorithms
- Add user rating functionality
- Expand dataset with more books
- Improve recommendation accuracy.
