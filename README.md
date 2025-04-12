# Toronto-Paramedic-Deployment-Optimization

The resources of the city of Toronto have been stretched thin under the strain of an escalating population size specifically impacting Toronto’s paramedic services. While it is known how many ambulances Toronto has, it is unclear how the city allocates its ambulances efficiently in order to satisfy the EMS call volume in any given forward sortation area (FSA). 

### Details

In this project, predictive and prescriptive analytics were leveraged to accurately predict the number of calls in any FSA on any day of the year. These predictions were then subsequently used to minimize the number of ambulance units needed to address these calls providing a comfortable buffer for Toronto’s paramedics should the actual call volumes suddenly spike. Using demographic data from the 2016 Canadian census and open-source Toronto paramedic call and station data, a linear regression model combined with feature engineering techniques was trained on the last 8 months of the year and tested on the first 4 months, producing predictions for the first four months of 2016. 

Next, a greedy algorithm was used to assign the calls based on closest proximity to their respective paramedic stations across Toronto. This was then inputted in an integer programming optimization problem that produced the minimal number of ambulances required at each station to satisfy those calls. It was found that using a standard linear regression model with an improved accuracy score of 50% over the benchmarked base mean call volume prediction accuracy, Toronto can satisfy its emergency calls using approximately 55 out of Toronto’s 242 total ambulances on a daily basis. It was also found that the winter season would require more ambulances than the spring. 

The model can therefore make efficient use of paramedic resources which could be allocated elsewhere. This result is well within the city’s resources and can thus adequately manage the rapidly growing city. 

