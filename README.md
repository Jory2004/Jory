## Here are 10 SQL queries you can run on KSA table in the movies dataset:

### 1. List all theaters
```sql
SELECT name, genre, location FROM movies.KSA;
```
### 2. Count the total number of theaters
```sql
SELECT COUNT(*) AS total_theaters FROM movies.KSA;
```
### 3. Find the highest-rated theaters
```sql
SELECT name, rating FROM movies.KSA WHERE rating = 5;
```
### 4. Find theaters with zero ratings
```sql
SELECT name FROM movies.KSA WHERE rating = 0;
```
### 5. Count theaters by genre
```sql
SELECT genre, COUNT(*) AS count FROM movies.KSA GROUP BY genre;
```
### 6. List theaters with more than 50,000 reviews
```sql
SELECT name, review_count FROM movies.KSA WHERE review_count > '50000';
```
### 7. Find theaters located in Saudi Arabia
```sql
SELECT name, location FROM movies.KSA WHERE location LIKE '%Saudi Arabia%';
```
### 8. Show theaters with missing best comments
```sql
SELECT name FROM movies.KSA WHERE best_comment IS NULL;
```
### 9. Find the average rating of theaters
```sql
SELECT AVG(rating) AS avg_rating FROM movies.KSA;
```
### 10. Find the most common theater genre
```sql
SELECT genre, COUNT(*) AS count FROM movies.KSA GROUP BY genre ORDER BY count DESC LIMIT 1;
```






