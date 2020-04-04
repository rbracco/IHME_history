# IHME Covid19 Prediction History

This is meant to keep a complete historical record of the predictions made by the [UW IHME Covid 19 Model](http://www.healthdata.org/covid). It is important that these records remain available to researchers and the general public so that we can know how well the model did and use this in the future to build better models.

## About the IHME UW Model:

The model was publicly released on Mar. 26th, 2020 without undergoing peer review. Publication link: https://www.medrxiv.org/content/10.1101/2020.03.27.20043752v1.full.pdf

### Listed Authors: 
  - [Christopher J.L. Murray](http://www.healthdata.org/about/christopher-jl-murray)

### Co-authors:
  - [Ali Mokdad](http://www.healthdata.org/about/ali-mokdad)
  - [Abraham Flaxman](http://www.healthdata.org/about/abraham-flaxman)

### Citation
>IHME COVID-19 health service utilization forecasting team. Forecasting COVID-19 impact on hospital bed-days, ICU-days, ventilator days and deaths by US state in the next 4 months. MedRxiv. 26 March 2020. doi:10.1101/2020.03.27.20043752.

### About the model:

#### Core Assumptions: 

The UW IHME model assumes that if the US follows 3 of the 4 following measures (school closures, closing non-essential services, shelter-in-place, and major travel restrictions) that they will "follow a trajectory similar to Wuhan, China". It assumes all US States will have implemented such policies by April 2nd. The authors chose not to include an increased mortality rate for Covid19 patients unable to receive medical care due to an healthcare system that is above capacity. 

#### Methodology:

With these assumptions as a starting point, the authors developed a curve-fitting tool to fit a nonlinear mexed effects model to the available admin I cumulative death data. The cumulative death rate for each location is assumed to follow a parameterized Gaussian Error Function. The estimates are produced using an ensemble of two models with this design. 

For the 23 states that were not yet beyond the threshold death rate of 0.31 per million (at time of model computation), estimations were made on when they were surpass this threshold based on the ratio of observed cases to deaths in the states that had already surpassed the threshold. 

Hospital service utilization was calculated using a microsimulation model by using the average age pattern from Italy, China, South Korea and the US. Hospital stay duration was estimated using the median time found elsewhere. Patients over 75 years of age were assumed to have a stay of 10 days while those under 75 were assumed to have a stay of 8 days. 

### Peer-review:

### Criticism:

I and others have expressed grave concern that the model was released to local, state and federal governments with no peer-review. Furthermore it appears that there has been little or no attempt to inform the public and policymakers of the questionable assumptions that underpin the model. The abstract and model FAQ make no mention of the strong assumptions and they are only included in the final 2 pages of the paper.

More below:

-[Rapid post-publication peer review by Prof. Carl Bergstrom](https://twitter.com/CT_Bergstrom/status/1244815009303023616)
-[The IHME Covid19 model is dangerously flawed (Disclaimer: I am the author)](https://medium.com/@robertbracco1/the-ihme-covid19-model-is-dangerously-flawed-c19928464db1)


## Data:

We have captured the model's estimations for the following dates:

-3/29/2020
-3/30/2020
-3/31/2020
-4/1/2020

We will capture data moving forward, but if you have access to the data releases from 3/26-3/29 please open an issue or [reach out on twitter](https://twitter.com/MadeUpMasters). 