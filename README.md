# Applied Statistics (Statapp) project
Realized with the joint participation of Keryann MASSIN (myself), Juliette VEILLON, Kilan ANDRU, and Xavier LACOUR.

**Objective**: Based on the socioeconomic and genetic data of an individual, is it possible to determine his global health?

**Tools and materials**: We used the databases from the Healh and Retirement Study, and explored it using various machine learning techniques such as XGBoost, RandomForest, Lasso, 2SLS and Within regression.


**Explanation of the project arborescence:**

*Repository 'pretreatment'*: it gathers all the first procedures we applied to the database, from simple cleaning to the implementation of a Lasso highly efficient in the handling of missing values.
- file_00: we looked for the best methods to potentially use, according to the Fragile Family Challenge.
- file_00: we merge the socioeconomic database and the genetic database into one dataset.
- file_01: we merge section A and E in genetic data.
- file_02: we drop spouses'related columns and columns with more than 65% of missing values.
- file_03: we delete health data and transform categorical data into dummy variables.
- file_04: implementation of the 'Lasso with High Missing Rate', namely 'HMLasso'.
- file_05: we impute remaining missing values.
- file_06: code helpful to select waves.

*Repositery 'Health_index'*: using t-Stochastic Neighbors Embedding algorithm, we summarized the health of an individual into one real number.
- file_01: we create the health index.
- file_02: we analyze its robustness and the way he behaves when an individual's whereabouts are changed a little.
- file_03: we proceed to descriptive statistics.

*2SLS*: we try a 2-stages least squares algorithm to see how this first linear method performs.

*Panel_estimates*: we apply a within regression to our data and try to predict the previously created health index.
- file_01: we apply the within regression.
- file_02: we check wether mathematical necessary hypothesis are verified to apply the within regression.

*Tree_methods*: we attempt tree based methods such as XGBoost and RandomForest to predict the health index.
- file_01: this file contains tries to see whether such methods are, at first glance, a promising path to follow.
- file_02: we apply XGBoost regressor and classifier.
- file_03: we apply Random Forest regressor and classifier.
- manipulate_data.py: a file that has been used to ease coding.

*Rapport*: the final report. The whole project is fully explained within the report.

*Soutenance*: the presentation we performed to conclude this project.


If you have any question, feel free to contact one of the previously mentioned authors.


