# Working-with-KSA-Entertainment-Data-Set-in-MySQL-from-Scratch


## For the following analysis I have use the project data set and the Table name is KSA_Entertainment

``` SQL
USE project;
```
## Q1. Identify the top tourist attractions with the highest number of reviews.
``` SQL
SELECT name, rating, review_count, location
FROM KSA_Entertainment
WHERE genre = ' Tourist attraction'
ORDER BY review_count DESC
LIMIT 5;
```
<img width="572" alt="image" src="https://github.com/user-attachments/assets/760ef0e9-287d-42dc-8eb3-0c183e85e3cb" />

## Q2. Retrieve the top-rated parks in Saudi Arabia with the highest ratings.
``` SQL
SELECT name, rating, review_count, location
FROM KSA_Entertainment
WHERE genre = ' Park' AND location LIKE '%Saudi Arabia%'
ORDER BY rating DESC, review_count DESC
LIMIT 5;
```
<img width="487" alt="image" src="https://github.com/user-attachments/assets/a9205593-230f-421c-a507-bcc1511b3f09" />

## Q3. Find all children's amusement centers in Dhahran, Saudi Arabia.
``` SQL
SELECT name, rating, review_count, location
FROM KSA_Entertainment
WHERE genre = ' Childrens amusement center' AND location LIKE '%Dhahran Saudi Arabia%';
```
<img width="487" alt="image" src="https://github.com/user-attachments/assets/ddc1726b-c39c-422d-8c64-ccd5b928b21d" />

## Q4. Find the best-rated museums in Saudi Arabia.
``` SQL
SELECT name, rating, review_count, location
FROM KSA_Entertainment
WHERE genre = ' Museum' AND location LIKE '%Saudi Arabia%'
ORDER BY rating DESC, review_count DESC
LIMIT 3;
```
<img width="354" alt="image" src="https://github.com/user-attachments/assets/458377ac-b3b5-4788-8d65-05f740e5c8de" />

## Q5. Find the highest-rated escape room center in Al Khobar, Saudi Arabia.
``` SQL
SELECT name, rating, review_count, location
FROM KSA_Entertainment
WHERE genre = ' Escape room center' AND location LIKE '%Al Khobar Saudi Arabia%'
LIMIT 1;
```
<img width="385" alt="image" src="https://github.com/user-attachments/assets/c33f928c-013f-4919-9299-8a2d146578ff" />





