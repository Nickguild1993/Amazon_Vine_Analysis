# Amazon Vine Analysis
## Overview  
The purpose of this analysis was to look at the the total number of reviews from one of a 50 datasets that we could choose from (I chose the dataset for video games) but specifically at the reviews that fell under the **"Vine"** program.  The Vine Program is a review based program that sellers pay Amazon for in order to secure (written) reviews from customers who have purchased their products.  The idea being that products with a high number of (hopefully) positive reviews will be purchased by future like minded customers over those that do not have a high number of written reviews.  However, there is a question of bias and incentivization when it comes to paying customers to write reviews.  Because they're getting a benefit in some form, do they feel obligated to write a review that makes the item out to be better than it actually is?  This may not even be a conscious decision on their part- they could be lavishing undue praise on the copy of *Skyrim* they bought without trying to skew the reviews- they just feel a sense of gratitude from receiving a gift from the Vine program and instead of giving the game 4 stars, they decide to give it 5 stars instead.

Therefore, we want to examine the reviews of individuals who're in the Vine program and compare them to the (much greater sample) of those customers who are not in the program but who also left reviews.  The goal is to see if there is a noticeable, significant difference between the reviews of Vine members and non-Vine members.

## Results: 

#### How many Vine reviews and non-Vine reviews were there?

- When filtering all reviews for those that received at least 20 total votes (as a way to select reviews that are more likely to be helpful/reliable), we had a total of 40,565 reviews, which can then be further broken down into the Vine reviews and the non-Vine reviews.

![Alt_text](https://github.com/Nickguild1993/Amazon_Vine_Analysis/blob/main/M16_Unwritten_DF.png)

- The above dataframe is comprised of all the non-Vine reviews, of which there were 40,471 (99.7% of the **total** 40,565 reviews in the dataset)

![Alt_text](https://github.com/Nickguild1993/Amazon_Vine_Analysis/blob/main/M16_Written_DF.png)

- The above dataframe is made up of all the individuals participating in the Vine program who wrote reviews, of which there are 94 reviews (which equates to 0.0023% of the **total** number of reviews in the dataset)


#### How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

- Of the <ins>94 Vine reviews, 48 of them were 5 star reviews</ins>, which means that the products reviewed by Vine participants recieved 5 star reviews over 51% of the time.

- There were of course many more non-Vine reviews, both in totality and in those that gave the product 5 stars.  Those figures are <ins>40,471 non-Vine reviews in total, with 15,663 of those earning 5 star status</ins>, for a 5 star percentage rating of 38.7%


#### What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

- The percentage of Vine reviews that were (rubber stamped) with 5 stars was 51%, while the percentage of **non**-Vine 5 star reviews given came in *much* lower, at 38.7%.



## Summary: 

Based on the rate of five star reviews for Vine participants (51% five star rate) compared to non-Vine participant five star review rates (38.7%) I believe a significant and meaningful bias exists on behalf of those using Vine to reward the products they're reviewing (whether they do so consciously or subconsciously) with a noticably higher rating than they would give, were they not being compensated for doing so.

In order to further support my theory, I ran an average of the `star_rating` for both the vine users and non-vine users DataFrames.  Below is an image of the results.

![Alt_image](https://github.com/Nickguild1993/Amazon_Vine_Analysis/blob/main/M16_avg_stars.png)

The average star rating really drives home the frankly stunning ratings difference between the two groups.  The **Vine Users** give an average review of 4.2 stars, while the **non**Vine Users give an average review of only *3.34* stars.  Clearly this program that Amazon is running is creating a competitive advantage for the companies that participate in it because the individuals who review their products are far more generous in their scores than those who're not compensated to do so.  In my opinion, in order to have a fair and balanced review system that can be universially trusted, the Vine program should be axed.

