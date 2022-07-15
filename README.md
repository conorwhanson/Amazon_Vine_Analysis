# Amazon Vine Review Analysis
The purpose of this analysis is to utilize PySpark, AWS Databases, and PostgreSQL to perform EDA on Amazon Vine reviews and filter data to discover if there is any bias in reviews of watches from Vine program subscribers. 

### Results
**Vine Reviews**
- There were a total of **47** Vine program reviews on watches.
    ![vine_reviews](https://github.com/conorwhanson/Amazon_Vine_Analysis/blob/main/resources/vine_reviews.png)

- Of the total reviews there were **15** 5-star reviews from Vine program subscribers.
    ![vine_5star](https://github.com/conorwhanson/Amazon_Vine_Analysis/blob/main/resources/vine_5star.png)

- This amounts to 5-star ratings making up **32 %** of total Vine reviews.

**Non-Vine Reviews**
- There were a total of **8362** non-Vine reviews.

![nonvine_reviews](https://github.com/conorwhanson/Amazon_Vine_Analysis/blob/main/resources/nonvine_reviews.png)

- Of the total reviews there were **4332** 5-star reviews from non-Vine subscribers.
![nonvine_5star](https://github.com/conorwhanson/Amazon_Vine_Analysis/blob/main/resources/nonvine_5star.png)

- This amounts to 5-star ratings making up **52 %** of total non-Vine reviews.

### Summary & Recommendations
The first thing to note in this analysis is the imbalance of total reviews between the Vine and non-Vine datasets. There are significantly more non-Vine reviews available comapred to the Vine reviews. This gives us a better picture of non-Vine reviews data set, but there are not enough data points to draw any concrete conclusions about the Vine review data set. With only 47 total Vine reviews for watches this the sample size is too small to explore potential bias in 5-star Vine reviews. Therefore, it is inconclusive if there is bias. 

However, further analysis could be done if more Vine reviews could be gathered. Further, I'd also recommend filtering the data by "Verified Purchase" to ensure the accuracy of the results. This would ensure that reviews are, in fact, written by those who purchased the watches. If more data points are gathered for the Vine reviews, then a comparison of Vine to non-Vine reviews based on verified purchase would be hepful to determine if any bias exists for watches with Vine reviews.