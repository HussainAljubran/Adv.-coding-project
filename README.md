# Working-with-KSA-Entertainment-Data-Set-in-MySQL-from-Scratch


## For the following analysis I have use the project data set and the Table name is KSA_Entertainment

``` SQL
USE project;
SELECT *
FROM KSA_Entertainment;
```
<img width="1041" alt="image" src="https://github.com/user-attachments/assets/e0c07253-3660-49b7-874c-e2c20839bf4e" />

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

## Q6. Retrieve all bowling alleys in Riyadh, Saudi Arabia.
``` SQL
SELECT name, rating, review_count, location
FROM KSA_Entertainment
WHERE genre = ' Bowling alley' AND location LIKE '%Riyadh Saudi Arabia%'
```
<img width="410" alt="image" src="https://github.com/user-attachments/assets/150da834-3583-4615-8c3f-6d26d4adb346" />

## Q7. Retrieve the best-reviewed tourist attractions in Jeddah, Saudi Arabia.
``` SQL
SELECT name, rating, review_count, location
FROM KSA_Entertainment
WHERE genre = ' Tourist attraction' AND location LIKE '%Jeddah Saudi Arabia%'
```
<img width="410" alt="image" src="https://github.com/user-attachments/assets/ad79d9e1-11a8-468a-98ee-1734e4418943" />

## Q8. Find the top-rated science museum in Al Khobar, Saudi Arabia.
``` SQL
SELECT name, rating, review_count, location
FROM KSA_Entertainment
WHERE genre = ' Science museum' AND location LIKE '%Al Khobar Saudi Arabia%'
ORDER BY rating DESC, review_count DESC
LIMIT 1;
```
<img width="410" alt="image" src="https://github.com/user-attachments/assets/09123bdc-81e7-433e-8b69-5f20127c8614" />

## Q9. Find the top-rated Movie theater in Saudi Arabia.
``` SQL
SELECT name, rating, review_count, location
FROM KSA_Entertainment
WHERE genre =  ' Movie theater' AND location LIKE '%Saudi Arabia%'
ORDER BY rating DESC, review_count DESC
LIMIT 5;
```
<img width="686" alt="image" src="https://github.com/user-attachments/assets/04fcc018-b970-4b72-a590-3ada6c114f4b" />

## Q10. Find the top-rated Movie theater in Dammam, Saudi Arabia.
``` SQL
SELECT name, rating, review_count, location
FROM KSA_Entertainment
WHERE genre =  ' Movie theater' AND location LIKE '%Dammam Saudi Arabia%'
ORDER BY rating DESC, review_count DESC
LIMIT 3;
```
<img width="686" alt="image" src="https://github.com/user-attachments/assets/6d885595-eda5-4e0e-9cba-e63949874b3e" />





