# MOVIE RECOMMENDATION SYSTEM
> Movie Recommendation System using PySpark, ALS, SQLLite (Movielens Dataset)

### REQUIREMENTS
---
- **`!pip install sqlite3`**
- **`!pip install pyspark`**

> **All of the required modules and libraries are listed below:**

- **for machine learning processes**
```
from pyspark.ml.evaluation import RegressionEvaluator
from pyspark.ml.recommendation import ALS
from pyspark.ml.tuning import TrainValidationSplit, ParamGridBuilder
```
- **for dataframe and spark session processes**
```
from pyspark.sql import SparkSession
from pyspark.sql.functions import * 
from pyspark.sql.types import *
from pyspark.context import SparkContext
from datetime import date, timedelta, datetime
import time
```


### MOVIELENS DATASET INFORMATION
---

- **ratings.csv**
```
userId, movieId, rating, timestamp
```
- **tags.csv**
```
userId, movieId, tag, timestamp
```
- **movies.csv**
```
movieId, title, year, genres
```
- **links.csv**
```
movieId, imdbId, tmdbId
```

### INFORMATIONS
---

- **The file hierarchy required for the code to work properly is as shown in the figure below:**

![readme için](https://user-images.githubusercontent.com/68853621/164267811-a2712fff-c3bb-4313-baef-7ae07b763002.jpg)


- **All the necessary directions for the code are explained in detail in the code, and the code is divided into certain sections as shown below according to its function:**

![readme2](https://user-images.githubusercontent.com/68853621/164268432-3f092997-0b88-42ea-b2ba-7ebae9a68b76.jpg)

### MOVIE RECOMMENDATION SYSTEM OUTPUT
---

> **Movie recommendation system that filters the User_Id information according to the user we want and lists the most compatible movies for that user.**

***Please edit the filter .filter("User_Id = N") with the user's ID (N) according to the user you want.***

![ex_system_output](https://user-images.githubusercontent.com/68853621/164270057-f9e6c690-8524-490a-8730-3b5cb7885fb2.jpg)
