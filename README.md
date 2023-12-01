# Amazon Vine Analysis

## Overview of the analysis
This project analyzes the Amazon Vine program and determines if there is a bias toward favorable reviews from Vine members. The analysis uses PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, load the transformed data into pgAdmin, and calculate different metrics. We focused on the US reviews for video games.

## Results

- How many Vine reviews and non-Vine reviews were there?
  - There were **4,291** Vine reviews 
  - There are **1,781,706** non-Vine reviews. 
<img width="576" alt="image" src="https://user-images.githubusercontent.com/58046234/163722447-235f9b5f-9c0a-44b4-97fd-79b93246fcca.png">
<img width="577" alt="image" src="https://user-images.githubusercontent.com/58046234/163722483-f85e2b9e-09c1-4655-9d50-73e99f4bc978.png">

- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
  - There were **1,607** Vine reviews with 5 stars. 
  - There were **1,025,317** non-Vine reviewers with 5 stars. 
<img width="574" alt="image" src="https://user-images.githubusercontent.com/58046234/163722747-50efae03-f427-41cd-8750-79d7cf834e1e.png">
<img width="559" alt="image" src="https://user-images.githubusercontent.com/58046234/163722658-9940bbac-214d-4f62-b975-1278d80bfdff.png">

- What percentage of Vine reviews were 5 stars? What percentage of non-vine reviews were 5 stars?
  - The percentage of Vine reviewers with 5 stars is about **57.55%**. 
  - The percentage of non-Vine reviewers with 5 stars is about **37.45%**.
  - Blow shows the results if they were paid.
<img width="658" alt="image" src="https://user-images.githubusercontent.com/58046234/163722901-8ee0f0f1-31ff-40ff-8138-43d78e933abc.png">

## Summary
57% of the reviews in the Vine program were 5-star reviews whereas the percentage in the non-Vine reviews is only 37%. This describes a positivity bias for reviews in the Vine program.
Additionally, we could analyze the mean, median, and other stats of the star rating for the Vine and non-Vine reviews.
