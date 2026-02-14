# Recommender System Demo using Matrix Factorization (SVD)
This notebook demonstrates a simple movie recommender system built with the Surprise library. It uses matrix factorization (SVD) to predict user–movie ratings and recommend top movies.

## Features

- **User-based Recommendations**: Get personalized movie recommendations for any user
- **Content-based Recommendations**: Find movies similar to a given title
- **Model Evaluation**: Cross-validation and performance metrics (Precision@5, Recall@5, RMSE)
- **Implicit Feedback**: Converts ratings to binary preferences (liked/not liked)

## Dataset

The system uses two CSV files (MovieLens Dataset downloaded form from GroupLens Research Lab - [Link](https://files.grouplens.org/datasets/movielens/ml-latest-small.zip)):
- `movies.csv`: Contains movie information (movieId, title, genres)
- `ratings.csv`: Contains user ratings (userId, movieId, rating, timestamp)

## Requirements

- Python 3.7+
- Dependencies listed in `requirements.txt`

## Installation & Setup

###  Clone the Repository

```bash
git clone https://github.com/prasadcam06-hub/Recommended-System-Demo.git
```

### Create Virtual Environment (Recommended)

```bash
# Create virtual environment
python -m venv movie_rec_env

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

## Usage

### Running the Jupyter Notebook

 **Start Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```

 **Open the notebook**: Navigate to and open `prasad.ipynb`

3. **Run all cells**: Execute all cells in order by selecting "Cell" → "Run All" or run each cell individually with `Shift+Enter`

### Running as Python Script

If you prefer to run the code as a Python script:

 **Convert notebook to Python script**:
   ```bash
   jupyter nbconvert --to script prasad.ipynb
   ```

 **Run the script**:
   ```bash
   prasad.ipynb.py
   ```

## Expected Output

When you run the notebook, you should see:

1. **Model Training Progress**: surprise.model_selection
2. **Evaluation Metrics**: 
   -RMSE: 0.8814
   -Precision@5: 0.6574
   -Recall@5: 0.4685


3. **Sample Recommendations**: Personalized movie recommendations for users 140,603,438
4. **Predict ratings for unseen movies for a specific user**: user 196.

