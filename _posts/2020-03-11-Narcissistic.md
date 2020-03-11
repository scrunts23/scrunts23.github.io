---
title: "Millennial’s: More Narcissistic than Other Generations?"
date: 2020-03-11
tags: [data wrangling, data science]
header:
  image: "/images/1_x0wDucR4cY8TDdZQlki5xw.jpeg"
excerpt: "Data Wrangling, Data Science, Messy Data"
mathjax: "true"
---


## Millennial’s: More Narcissistic than Other Generations?

**Brief History Lesson in Greek Mythology:**

Narcissism as a personality trait is generally conceived as excessive self-love. In Greek mythology, Narcissus was a man who fell in love with his reflection in a pool of water who disdained those that loved him, even causing the individuals around him to take their own life to prove their devotion to his striking beauty. Thus, giving us the modern-day term of Narcissism from his personality traits.

**Introduction to the NPI Survey:**

![](https://cdn-images-1.medium.com/max/5458/1*XLy6FzJW1GfSboJujn-0Ag.jpeg)

The NPI (Narcissistic Personality Inventory) was developed by Raskin and Hall (1979) for the measurement of narcissism as a personality trait within social psychological research. It is based on the definition of narcissistic personality disorder found in the DSM-III (*Diagnostic and Statistical Manual of Mental Disorders Vol 3)* but this is not a diagnostic tool for Narcissistic personality disorder (NPD) and instead measures sub-clinical or social expressions for narcissism. So, even someone who gets the highest possible score on the NPI does not necessarily have NPD. The NPI consists of forty pairs of statements that should be carefully selected to best reflect one’s personality.

**Data Processing:**

Upon initial investigation of the NPI assessment results, the data frame included 11,243 entries:

· Gender data for everyone that completed the NPI assessment

· Age of individuals that completed the NPI assessment (ages below 15 were omitted in the data collection process)

· Score for each paired question (n = 40)

· The total score for the NPI assessment (range of 0–40)

· Time elapsed for taking the NPI assessment

The next step was to filter the data to find if there were any outliers present within the age distribution. From this step, it was found that it was necessary to omit a portion of the NPI assessment results to ensure the age distribution was between 15–100 years old.

![Identifying age outliers in with the data](https://cdn-images-1.medium.com/max/2000/1*ayerkZKzAWePqFEBpRwUuQ.png)

Once the data was processed, the sample size resulted in 11,009 individuals that were within the age range of 15–100 years old. The next step was to create Generation data based on the ages of the individuals that completed the NPI assessment. The break down of Generations are below:

· Generation Z (15–25 years old)

· Millennials (26–40 years old)

· Generation X (41–55 years old)

· Baby Boomer Generation (56–74 years old)

· The Silent Generation (75–100 years old)

**Initial Data Exploration:**

Using the processed data, histograms were created to show the overall distribution of scores with the number of NPI assessments taken. As seen below, the average score is approximately 13.2.

![](https://cdn-images-1.medium.com/max/2000/1*02j961qstF3h8zZBe9ygcA.png)

With having gender categories within the original data set the next step would be to break down the distribution of scores based on gender (Male, Female, and other Genders):

![](https://cdn-images-1.medium.com/max/2000/1*cnRXrJa-ujsc2QoVFfd0Jg.png)

![](https://cdn-images-1.medium.com/max/2000/1*zuetiM3dTkhQ2ola4axvRQ.png)

![Distribution of Scores based on Gender](https://cdn-images-1.medium.com/max/2000/1*cB-NDJZL-po7HNftzBDTrQ.png)

As expected, the average of each gender roughly mimics the overall distribution of scores. The male category results show an average score of 14.1 with a sample size of 6,310. Looking at the other gender labeled classification also has an average score of 14.1 but has a much smaller sample size of 34. Turning to the female category, they result in an average score of 11.9 with a sample size of 4,665. The results of the distribution of scores by gender show that women tend to have lower narcissistic tendencies compared to the other two gender categories.

**Which Generation is More Narcissistic?**

Using the Generation data that was created in the data processing step the next step would be to create a density plot to show the overall distribution of scores based on Generations to answer the question of which generation has higher narcissistic traits based on the NPI assessment.

![Density plot for scores based on Generations](https://cdn-images-1.medium.com/max/2000/1*lWTiV-3zWx3T_DtDACWadQ.png)

Based on the graph above, you can see that The Silent, Baby Boomer and Gen X Generations share similar trends with an average score below 10 and both Gen Z and Millennials share similar trends with a higher average score closer to the whole samples mean. Based on the overall distribution, Generation Z on average has more individuals with higher narcissistic tendencies. The next step is to look at the breakdown of the genders and generation data together to see if it shows a similar trend to the overall generation density plot.

![](https://cdn-images-1.medium.com/max/2000/1*E8tAC7CYBRDSjj3UkQn3NA.png)

![](https://cdn-images-1.medium.com/max/2000/1*cFL5NNyB2OIzSiIush5lUg.png)

![Density plot of Scores based on Generations for Males, Females and Other Genders](https://cdn-images-1.medium.com/max/2000/1*ZPn9Mndin7mzH9YIVaEbhw.png)

Similar to the histograms above, one can interoperate that the males within this data set show that they have higher narcissistic tendencies based on the NPI assessment answers. Each plot, especially the male and female plots; shows that individuals within the Generation Z have a higher number of people with higher NPI assessment scores. The density plot for the labeled category of other genders is skewed due to the lower amount of individuals who identify as other genders.

**Deeper Dive into the Generation Data:**

From the analysis of the distribution of scores overall and the generation distribution scores based on gender types, the next step is to take a deeper look at the breakdown of the number count of individuals within a set score range.

![Heat map of Scores based on Generations](https://cdn-images-1.medium.com/max/2000/1*AF2VgzZJOn6iqxfrrSXAfQ.png)

From the comparison of the overall non-gender specific density plots and heat map, we do confirm that Gen Z individuals as a whole, have a higher number of participants that score higher based on their assessment scores.

![Heat map of Scores based on Generations for Males](https://cdn-images-1.medium.com/max/2000/1*BKjTgAMBAEesiub6KSLdKA.png)

From the interpretation of the male generation distribution, male individuals within Generation Z have a higher average score from the NPI assessment.

![Heat map of Scores based on Generations for Females](https://cdn-images-1.medium.com/max/2000/1*N8qhgTd9wJpH8b8Qlxypug.png)

Looking at the breakdown of the females within the dataset we can confirm that most of the females fall within the calculated average of 11.9. Similar to the males, the females also share a trend in that Generation Z on average has a higher collection of individuals with higher narcissistic tendencies.

![Heat map of Scores based on Generations for Other Genders](https://cdn-images-1.medium.com/max/2000/1*0hwuYxtl2ikoB7rDN3OfVg.png)

With the Gender that is labeled as other, the distribution is confirmed the majority of the individuals fall within the calculated average score of 14.1. With this gender group, it is hard to see a similar pattern to the other gender groups due to the lower number of individuals within the other gender category.

**Conclusions: Who is more Narcissistic?**

Based on the information within this sample data it was found on average those who completed the NPI assessment, it is determined that Generation Z and Millennials have higher narcissistic tendencies based on scores of the NPI assessment questions. From the heat maps analysis across all studied gender groups, individuals that fall within Generation Z would show more narcissistic tendencies especially males that fall within this Generation.

![](https://cdn-images-1.medium.com/max/2000/1*Rz8ym3nJ1YPjSee2Rdr5gQ.jpeg)

**What is Next:**

This dataset contains many possibilities that could lead to various data exploration and modeling. Some items that could be looked into in the future include:

· Does the time that is taken to affect the overall score of assessment?

· Can I predict scores/age/gender based on the time elapsed on the NPI assessment?

Link to GitHub Repository [here](https://github.com/scrunts23/Unit-1-build-).

Note this is a project for Lambda School within the Data Science track.

Sources:

Raskin, R.; Terry, H. (1988). “A principal-components analysis of the Narcissistic Personality Inventory and further evidence of its construct validity”. Journal of Personality and Social Psychology, Vol 54(5), 890–902.
