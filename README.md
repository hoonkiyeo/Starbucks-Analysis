# Relationship between number of Starbucks and Prosperity

## Introduction and Hypothesis

- Starbucks was first established in Seattle at 1971. Fifty years later, there are about 25,000 stores around the world, and Starbucks has become an important culture beyond just a cup of coffee. In urban area like Chicago and New York, we can easily see the Starbucks in every block but it is hard to see in the rural area. By observing this kind of situation, our group came up with a simple question: “what makes the difference?” Our group think that the number of Starbucks stores could be one of the indicators that represent the prosperity of city or country. To check our claim, we made a hypothesis: null hypothesis with “there is no relationship between the number of Starbucks stores and the indicators that represents the prosperity of city or country” versus the alternative hypothesis with “there is some relationship between the number of Starbucks stores and the indicators that represents the prosperity of city or country”. In other words, we set our hypothesis H0 : Bj = 0 and Ha : Bj ̸= 0. Note that we used 7 variables including
“GDP”, “Happiness Score”, “Cost of Living”, “Rent Price”, “Quality of Life”, “Safety index” and “Population”.

- We expect Starbucks could be one of the important and indescribable index if our research has a meaningful result. In order to conduct our research, we first cleaned the data collected from variety sources and tested our hypothesis.


## Dataset

- We used the total of six datasets for this project.
- The first data we used is directory.csv from https://www.kaggle.com/starbucks/store-locations. This dataset includes a record for every Starbucks or subsidiary store location in operations worldwide. This data was scraped from the Starbucks store locator webpage by https://github.c om/chrismeller/. There are a number of including Brand, Store Number, Store Name, Owenership Type, Street Address, City, and Country.
- The second data we used is cost_of_living.csv from https://www.kaggle.com/dumbgeek/countries- dataset-2020?select=Cost+of+living+index+by+country+2020.csv updated by Varun Yadav. This dataset includes various variables such as cost of living and rent of each countires worldwide counted as the index number.
- The third dataset we used is quality_of_live.csv from https://www.kaggle.com/dumbgeek/coun tries-dataset-2020?select=Quality+of+life+index+by+countries+2020.csv updated by Varun Yadav. This data includes variables realted to the indicators of the overall quality of live such as safety index, health care index and quality of life index.
- The fourth dataset we used is happiness.csv from https://www.kaggle.com/unsdsn/world- happiness?select=2017.csv. There are two significant indicators in this dataset, which are happiness ranking of the countries worldwide and the happiness score of the those countries. These happiness scores and ranking use data from the Gallup World Poll. The happiness scores are entirely based on answers to the main life evalution question answered by respondents asked in the poll and the happiness ranking are assgined to each countries based on the scores.
- The fifth dataset we used is economic.csv from https://www.kaggle.com/nottisani/worldwide- economics-gdp updated by Gabriela McDavid. The dataset includes a number of variables that help us to get a sense of the economic status of countires worldwide such as the net GDP and the size of the population.
- The last dataset we used is gdpstate.csv from https://www.bea.gov/data/gdp/gdp-state.

## Analysis & Results

- After cleaning the dataset, our group mainly used “linear regression” for the analysis so that we are able to observe the dependency between the number of Starbucks and other variables. Our group checked whether there is a relationship between specific variables and number of Starbucks, we checked the associated p-value and found that only “GDP” and “Population” seemed meaningful for initial hypothesis. Hence, we made deeper analysis on both “GDP” and “Population”. We then used R-squared to check the fitness of our model. Moreover, our group detected that the number of Starbucks in USA seems to be too large compared to other datasets and therefore, we decided to subdivide the “USA” into “each states” to prevent USA being an outlier in terms of the number of Starbucks. Furthermore, to help the audience look our data at ease, our group used Choropleth map to compare the distribution of Starbucks in USA and GDP at glances. As non-linearity of the response-predictor relationship is one of the main concern in linear regression model, our group also checked whether there is a non-linear association with each variables to check which model is suitable by checking the associated p-value.

### Linear regression

![151747394-a146ec77-c6c5-4e29-9755-210887339fec](https://user-images.githubusercontent.com/69660509/176988646-2feaeec6-b0fa-498b-8fdf-779dc3198a53.png)


![151747461-313f639b-78ef-43ba-aa88-910f982a124e](https://user-images.githubusercontent.com/69660509/176988634-41ab631c-6f2a-4ca6-8865-22ed27a4745e.png)

<img width="700" height="400" alt="Screen Shot 2022-07-02 at 12 57 25 AM" src="https://user-images.githubusercontent.com/69660509/176988609-1f62c17b-d2ef-465a-bb53-032f13787228.png">

### Choropleth map

![12](https://user-images.githubusercontent.com/69660509/176988676-a7dbb5f9-a443-4da8-a94e-3df50fab9e8c.png)

![23](https://user-images.githubusercontent.com/69660509/176988688-dc7a838b-f6c9-4fd2-a6f3-2407e12bc394.png)

## Conclusion

- We were interested in the relationship between the number of starbucks stores and other various countries’ data. Then, we found out that United States had overwhelmingly many starbucks stores compared to other countries, so as a country scale, including United States in the data had the possibility of distorting data. Accordingly, we separated United States and delved into it in a more domestic and microscopic way. According to subsequent linear regression analyzing the correlation between the number of starbucks stores with other predictors on a U.S. state level, we discovered that ‘GDP’ was the most explanatory predictor. We found out the relation with GDP using linear regression model and geographic visualizations. Back to a country scale excluding United States, ‘GDP’ and ‘Pouplation’ of countries had higher correlation with the number of starbucks stores according to linear regression model. To quench our curiosity, we also went on to check non-linear association and re-confirmed that ‘GDP’ and ‘Population were still statistically significant. We have done by dissecting this project into two parts: United State’s domestic level, and international level. By looking at U.S. domestic level and international level with United States, GDP was assumed to be the strong predictor correlated with the number of stores. Of course, there existed limitation on these results. The number of stores in starbucks dataset was not accurate, due to missing countries (Italy) and wrong data inputs. Also, the correlation we found is not equivalent to causality. Therefore, more explanations and further analysis has to be done. Also, off the top of our head, we intuitively can predict that the more prosperous and richer the region or country is, the more starbucks stores located at. Though there was not a novel discovery in our project, it is an undeniable fact that ’GDP’ is the powerful predictor correlated with the number of starbucks stores. To sum up, in terms of the indicators of
‘GDP’ and ‘population’ we were able to reject the null hypotheses.