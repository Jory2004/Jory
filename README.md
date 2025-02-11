## Here are 10 SQL queries you can run on KSA table in the movies dataset:

### 1. List all theaters
```sql
SELECT name, genre, location FROM movies.KSA;
```
![image](https://github.com/user-attachments/assets/da6dc11f-e242-4a5e-9d8e-060f6d017d81)

### 2. Count the total number of theaters
```sql
SELECT COUNT(*) AS total_theaters FROM movies.KSA;
```
![image](https://github.com/user-attachments/assets/42a714c6-c8e0-4571-a0d6-f4e8ce29fb54)

### 3. Find the highest-rated theaters
```sql
SELECT name, rating FROM movies.KSA WHERE rating = 5;
```
![image](https://github.com/user-attachments/assets/54176d29-6097-4135-974f-e0bf1127d5de)

### 4. Find theaters with zero ratings
```sql
SELECT name FROM movies.KSA WHERE rating = 0;
```
![image](https://github.com/user-attachments/assets/ff04ff47-6e18-40e4-b7e8-bdcdec50e5c3)

### 5. Count theaters by genre
```sql
SELECT genre, COUNT(*) AS count FROM movies.KSA GROUP BY genre;
```
![image](https://github.com/user-attachments/assets/179261b0-d598-4a52-8366-5b4878e91cc8)

### 6. List theaters with more than 50,000 reviews
```sql
SELECT name, review_count FROM movies.KSA WHERE review_count > '50000';
```
![image](https://github.com/user-attachments/assets/c67ff2c9-4f0f-4330-8b5e-cbae7598f9a0)

### 7. Find theaters located in Saudi Arabia
```sql
SELECT name, location FROM movies.KSA WHERE location LIKE '%Saudi Arabia%';
```
![image](https://github.com/user-attachments/assets/a2b41dc8-5cdb-4381-b444-51e7658ecfc4)

### 8. Show theaters with missing best comments
```sql
SELECT name FROM movies.KSA WHERE best_comment IS NULL;
```
![image](https://github.com/user-attachments/assets/5a04a5b7-e47a-4b11-9ae1-3296e933cd95)

### 9. Find the average rating of theaters
```sql
SELECT AVG(rating) AS avg_rating FROM movies.KSA;
```
![image](https://github.com/user-attachments/assets/25c83a33-bf53-42d8-9747-229028ca44d2)

### 10. Find the most common theater genre
```sql
SELECT genre, COUNT(*) AS count FROM movies.KSA GROUP BY genre ORDER BY count DESC LIMIT 1;
```
![image](https://github.com/user-attachments/assets/b1f9038b-ae63-45fe-9c46-c23ca8ba6364)







