# Detection of housing-health relationship
How does the quality of housing we are living in affect our health? Which housing properties are affecting health the most (if any)? Are there some targeted measures that could increase both our quality of living and health status?

To answer some of these questions, we will do observational study based on a survey made by Mexican National Institute of Statistics and Geography in 2017. The National Household Survey (ENH) is carried out with the purpose of knowing the characteristics of the housing units; sociodemographic data about the household members, their occupation, education; as well as the availability of information and communication technologies goods and services in households.

First of all we will define a health variable in order to represent the current health status of each person. The health variable is based on 18 health related questions such as physical ability, ability to hear and see, frequency of pain and fatigue and the level of depression. Adequate normalized weight has been assigned to each of these variables. The maximum score of 18 represents a person completely healthy based on the studied health problems.


![Historgram](/img/histogram.png)

## House Problems vs health score

In following four figures we present the relation between four house variables and health variables. The habitants of the house were questioned whether the house is in need of a certain repair. They could either answer yes or no to these questions. Slight difference between these to groups is observed. One can see that in most of the cases house with need for a repair (blue bars) exhibit slightly lower values of health score. One has to have in mind that the distribution of health score is imbalanced across the population since most of the population is healthy so even a slight difference in health score could be important. In further analysis we will try to answer whether this difference is statistically significant. Interestingly it seems that people in badly maintained houses seem to be less depressed and nervous.

![Wall](/img/walls.png)
![Roof](/img/roof.png)
![Electrical](/img/electrical.png)
![Water pipes](/img/water.png)

## Bulding materials vs health

In the following two figures we present the relation between house materials and health variables.

The first figure relates the health score with roofing materials such as: waste material, cardboard sheet ,metal foil, asbestos sheet, palm or straw, wood or tile, roof with beams, roof tile, concrete slab.

![Roof material](/img/roof_m.png)

The second figure relates the health score with flooring materials such as: earth, cement or firm, wood mosaic or other coating.

![Floor material](/img/floor_m.png)

## Cell phone availability vs health

In the following figure we compared our health score with cell phone availability.

![Cell phone](/img/cellphone.png)


## Age of person vs health

In the following figure we compared our health score with the variable age in the dataset.

![Age person](/img/age.png)

The decreasing trend in health is clear, it is also expected since older people are usually less healthy.

## Linear regression
In our first regression model we used as predictor variables our health score previously generated, as predictor variables we considered only those derived from the data housing dataset.  
FIGURE 1
The regression shows that the following variables have a positive correlation ( the highest are cited  in decreasing order ) with the health score: fixed phone availability, walls that need no repair, roofs that need no repair, water pipes that need no repair. The regression also shows that the following variables have a negative correlation ( the lowest are cited in decreasing order ) with the health score: presence of a bedroom, socioeconomic factor and fuel type firewood.

In our second regression model we used as predictor variables our health score previously generated, as predictor variables we considered all the variables present in the house and person dataset.  
FIGURE 2
The regression shows that the following variables have a positive correlation ( the highest are cited  in decreasing order ) with the health score: relationship type, roofs that need no repair, water pipes that need no repair. The regression also shows that the following variables have a negative correlation ( the lowest are cited in decreasing order ) with the health score: sex, fuel type firewood, fuel type tank gas and having no relationship.

![Regression](/img/regression.png)

## The team
![The team](/img/avatars.png)