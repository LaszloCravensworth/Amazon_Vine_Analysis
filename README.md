# Amazon_Vine_Analysis

## Overview of Project
&nbsp;&nbsp;&nbsp; The purpose of this project was to analyze the written reviews by members of the paid Amazon Vine Program.  The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Out of the approximately 50 datasets, the Home Improvement category was selected for this analysis.  Pyspark was used to perform ETL (Extract, Transform, Load) of the data.  The data was loaded into an Amazon Database instance (AWS RDS).  The transformed data was loaded into pgAdmin.  In the summary section, the data is analyzed to see if there is bias toward favorable reviews from Vine members in the dataset.

## Resources
&nbsp;&nbsp;&nbsp;* Data Source: https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Home_Improvement_v1_00.tsv.gz

&nbsp;&nbsp;&nbsp;* Software: AWS, pgAdmin4, SQL, Google Colab, Jupyter Notebook

## Results

Code showing the databases created:
<br />
https://github.com/LaszloCravensworth/Amazon_Vine_Analysis/blob/main/Amazon_Reviews_ETL.ipynb
https://github.com/LaszloCravensworth/Amazon_Vine_Analysis/blob/main/Vine_Review_Analysis.ipynb

*How many Vine reviews and non-Vine reviews were there?
&nbsp;&nbsp;&nbsp;There was a total of 266 Vine reviews and 38,829 non-Vine reviews.
<br />
<p float="left">
  <img src="https://github.com/LaszloCravensworth/Amazon_Vine_Analysis/blob/main/pngs/total_vine_reviews.png" width="300" />
  <img src="https://github.com/LaszloCravensworth/Amazon_Vine_Analysis/blob/main/pngs/total_non_vine_reviews.png" width="300" /> 
</p>
<br />

*How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
&nbsp;&nbsp;&nbsp;There was a total of 125 5 star Vine reviews and 18,246 non-Vine 5 star reviews.
<br />
<p float="left">
  <img src="https://github.com/LaszloCravensworth/Amazon_Vine_Analysis/blob/main/pngs/five_star_vine_reviews.png" width="300" />
  <img src="https://github.com/LaszloCravensworth/Amazon_Vine_Analysis/blob/main/pngs/five_star_non_vine_reviews.png" width="300" /> 
</p>
<br />

*What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
&nbsp;&nbsp;&nbsp;There was a total of 46.992% 5 star Vine reviews and 46.990% non-Vine 5 star reviews.
<br />
<p float="left">
  <img src="https://github.com/LaszloCravensworth/Amazon_Vine_Analysis/blob/main/pngs/percentage_vine.png" width="300" />
  <img src="https://github.com/LaszloCravensworth/Amazon_Vine_Analysis/blob/main/pngs/percentage_non_vine.png" width="300" /> 
</p>
<br />

## Summary
&nbsp;&nbsp;&nbsp; Taking a look at the data it would appear that the percentage of 5 star reviews from Vine and non-Vine members is nearly identical.  Since the Home Improvement category was chosen, it could be that home owners and Vine members see eye to eye on outstanding products. With this being just one dataset among many categories, it would appear more data is needed to draw a conclusion either way.  From this data, there is little bias one way or the other.  One additional and likely useful analysis to perform, would be on the verified purchase column.  This would help eliminate any erroneous reviews.
