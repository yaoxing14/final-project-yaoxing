# Executive Summary

**Research Question**  

What characteristics of pets make them more likely to find new homes?

**Data**  

I'm from the full Austin Animal Center dataset (`aac_intakes_outcomes.csv`), which has intake and outcome details for about 79,000 cat and dog events. To keep things manageable, I picked 10 key columns (like animal type, intake method, and days in shelter) and randomly pulled 5,000 records into `data/aac_small.csv`.

**Methods**  

- **Exploration**: I made bar charts to compare adoption rates by pet type, breed, and whether they were neutered on arrival. Then I used boxplots to see how long adopted vs. non-adopted pets stayed. I also built simple tables to check intake method against adoption outcomes.  

- **Modeling**: Finally, I ran a logistic regression (`glm(family = "binomial")`) with all those predictors to see which factors really move the needle on adoption odds.

**Key Takeaways**  

- Neutered pets, healthy-looking arrivals, and shorter shelter stays tend to get adopted more often.  
- Breed and age still matter,puppies and kittens seem to catch people’s eyes first.  
- Whether an animal came in as a stray or a surrender also makes a noticeable difference in adoption chances.

