# Book recommendation engine

This is a book recommendation engine. The data used is reviews retrieved from Amazon and information about books from Google Books. 
The methods used are matrix factorization and collaborative filtering. The results are 20% better than the baseline (average rating the user gives).

## Details about notebooks
- `Code/eda-for-book-recommendation-dataset.ipynb` - exploring the dataset downloaded from kaggle, cleaning the data
- `Code/non-personalized-book-recommendations.ipynb` - giving non-personalized book recommendations for cold start: books that are popular and have good reviews and books that are liked often with the books the user already reviewed positively
- `Code/scraping-for-book-descriptions-100-books.ipynb` - choosing 100 most popular books and scraping information for them using Google Books API
- `Code/creating_user-book_matrix.ipynb` - creating a pivot table that contains a rating that every user gave to every book or null if they didn't review the book; normalizing that matrix so that the average rating for every user is zero
- `Code/collaborative-filtering-for-book-recommendations.ipynb` - user-user collaborative filtering
- `Code/matrix-factorization.ipynb` - matrix factorization for user-book matrix
- `Code/cross_validation.ipynb` - cross-validating matrix factorization and collaborative filtering, comparing to average rating the user gives
