Data Science in Practice(COGS108)

Project Summary: Fragrantica is a online fragrance encyclopedia platform where customers explore notes, brands, and share ratings and reviews on over hundred thousands of perfumes. Our research question was, Does the presence of specific fragrance notes (e.g. citrus, floral, woody, oriental) correlate with higher user ratings of perfumes on Fragrantica? (data collected from fragrantica.com)

We initially hypothesized that fragrances dominated by “heavy” notes (e.g., leather, oud, wood) would have lower average ratings, whereas fragrances with “fresh” notes (e.g., citrus, green tea, orange blossom) would have higher average ratings. However, our results indicate that the reality is quite the opposite. The average rating for perfumes with heavy notes was 4.04, compared to 3.97 for fresh-note perfumes, only marginally above the dataset average. 
Our EDA has supported this conclusion with the t-statistic results:
(t = 12.132, p < 0.001) - Heavy Notes
(t = 4.213, p < 0.001) - Fresh Notes
This indicates that, although both are statistically significant, there is a higher positive correlation for heavy notes. During our Lasso Regression, oud, and woody notes all appeared in the positive tail of the coefficient distribution, while most fruity and delicate floral accords appeared in the negative tail, further reinforcing our result.
We also expected that specific fragrance notes would appear together more often than by chance (e.g., green tea and citrus). To test this, we analyzed the top 20 most commonly occurring notes, calculating the Pearson correlation coefficient for each pair to determine whether the presence of one note is positively correlated with the presence of the other. 

This analysis enabled us to determine how frequently these combinations are used, compared to their use in independent occurrences. Our results revealed that there is a weak positive correlation between the pairs, with the highest correlation being (0.177) for jasmine and rose, followed by jasmine and musk (0.127), and jasmine and sandalwood (0.120). 

My Contributions: I worked on prior work on this reseach topic, looking at primary literature papers on what ML and statiscial methods has been preivosly used. After we got an idea on how to approach, I cleaned and normalized raw Fragantica data, from around 70k rows to 27k rows. Structured the data frame so we get top, middle and base notes in addition to ratings next to it. For our given hypyothesis I ran statistical tests, independent t-tests, to look at which notes are associated with higher ratings. I later on worked on to finalize our findings and complete checks on our project.
