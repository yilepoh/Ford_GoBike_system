# Ford GoBike System Data Investigation
## by Yi Le POH


## Dataset

### Structure of dataset

The dataset consist of 519,700 entries, entries are made when a user uses Ford GoBike. Each entry records the user's information and the user's activity. Each entry has 15 features. The features are as below:
- duration
- start time
- end time
- start station location (latitude, longitude, name, id)
- end station location (latitude, longitude, name, id)
- bike id
- user type
- member birth year
- member gender

We have derived additional variables from the station coordinates. The derived features are as below:
- region
- distance

In this dataset we have excluded missing information and inconsistent information. We have excluded 78,913 entries of data, leaving us with 438,087 entries.

The variables in the dataset have been assigned to the correct datatype. The time variable has been assigned labels to aid visualisation.

### Main feature(s) of interest in dataset

In this project, we assuming the role of a data analyst that is part of a marketing team in Ford GoBike. 

Our primary objective is to better understand the demographics and the behaviour of our users. With these insights, we can design advertising campaigns accordingly, capturing more new users and retaining existing subscribers.


## Summary of Findings

We categorise our findings in terms of GoBike user behavior and GoBike user demographics.

In terms of user demographcis, we found that:
- majority of the GoBike users are males. The GoBike male to female user ratio is 3:1
- majority of the GoBike users are from San Francisco (80%), followed by East Bay and San Jose. 
- majority of GoBike users are subscribers who paid monthly membership
- GoBike customers account to approximately 10% of the GoBike user base
- majority of the user base is between the age of 25-35.

In terms of user behaviour, we found that:
- GoBike users use GoBike for an average duration of 10 mins (600 sec)
- GoBike users are less likely to use GoBike above 30 minutes (1,800 sec)
- GoBike users use GoBike for an average travel distance of 1 km
- GoBike users are less likely to use GoBike to travel more than 2 km
- GoBike users tend to use GoBike more on weekdays
- GoBike users tend to use GoBike during peak hours: between 8-9am and 5-6pm
- GoBike users tend to use GoBike lesser at the end of the year (effect of season on the usage)

Looking at both user demographics and user behaviour, we found that:
- GoBike usage duration has a positive relationship with the usage distance, especially the upper limit of the usage distance
- rough estimate that GoBike users are able to cycle up to speed of 15 km/h
- GoBike user age has no obvious relationship with the user behaviour (usage duration and distance)
- GoBike user gender has no obvious relationship with the user behaviour (usage duration and distance)
- GoBike user region has an impact on the usage distance, where San Francisco has greater distance on average, followed by East Bay and San Jose
- GoBike user region has an impact on the usage duration, where San Francisco has the greatest usage duration on average, followed by East Bay and San Jose
- GoBike user type has a large impact on the user behaviour
    - GoBike subscribers, in general uses GoBike for shorter duration and distance
    - GoBike subscribers, in general uses GoBike for longer duration and distance
- Time has an impact on user behaviour
    - GoBike users tend to use GoBike less during weekends
    - GoBike users tend to use GoBike for longer periods of time during weekend
- Time has an impact on the user type
    - Subscribers tend use less GoBike on weekends, as compared to weekdays
    - Pool of customers that uses GoBike is fairly constant with time


## Key Insights for Presentation

The presentation focused on understanding our user. We started with the trend in user behaviour followed by user demographics and time. After that, we moved to undertanding the effect of user demographics on the user behaviour.

The presentation started with understnading GoBike user behavior in terms of usage duration and distance. We looked at the relationship between the usage duration and distance as a whole. This allows a general understanding of the users' perception of GoBike as a product.

The presentation then moves towards depicting the user demographics, such as gender, region and type. As we look into the age variable, we factor in the user type into the picture to start to show the audience that we have 2 very different user base, namely: subscriber and customer.

After that, we introduce the factor of time into the picture together. We look at the impact of time on the user behaviour. We left out some intermediate plots, and showed that time has an impact on the user behaviour. But not all users are equally affected.

We then looked into the impact of age on the behaviour while still showing the two different group of user type. By this time, we want to let the audience know that, the two groups of user type is very clear in terms of their behaviour. Age on the other hand has no impact on the behaviour. Presentation is finished with an interesting observation that duration is affected by the time of the day as well as the user region.

In the presentation, we left out the member gender as it has no direct effect on the user behaviour. we also left out some exploratory plots that leads us to the findings. We know that age has no direct impact on the user behaviour. But it can serve as a good variable to showcase the difference in user behaviour between different user type.
As for color, we stick to 'Blues' for different user types and 'Greens' for different user regions, for a consistent understanding. 