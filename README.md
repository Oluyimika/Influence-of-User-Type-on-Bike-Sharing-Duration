# (Bike-Sharing Data Exploration)
## by (Oluyimika Sosanya)


## Dataset

> This data contains information about individual rides made in a bike-sharing system covering 
the greater San Francisco Bay area in 2019, including duration, user type, start time and end time, and other trip attributes. 
The dataset can be found following links from [this page](https://s3.amazonaws.com/baywheels-data/index.html)
with feature documentation available [here](https://www.lyft.com/bikes/bay-wheels/system-data).

> I downloaded the 12 data programatically for a full year's coverage, merged them to form a master dataset,
and performed some data wrangling to get it ready for exploration. The master data set has about 2,410,000 entries.
Before starting my exploration I feature engineered new period columns (time of day, day of week, and month) from the 
start time attrobute to make my analysis easier.


## Summary of Findings

> In the exploration, I found that there was a strong relationship between the
duration of individual rides and user type, with modifying effects from the time of day,
day of week, and month variables associated with bike rides.

> In univariate exploration, when outliers were removed I found that duration takes a long-tail
distribution with most trips on the short end between 250 and 750 secs. The exploration also showed that
Subscribers were the largest users of the scheme, accounting for over 80% of individual rides analyzed.
The short duration might be connected with the fact that most trips covered a short distance, with frequent
trips between stations.

> With bivariate exploration, I found some interesting relationships between duration and user type with 
time of day, day of week, and month. While subscribers used the scheme more, customers trip lasted for longer durations.
While most trips were taken on weekdays, the weekends saw longer trip duration.

> After establishing the interaction between duration and user type with the period variables (time, day, and month),
I used multivariate exploration to explore the impact of user type on duration and the three levels of period variables.
I found that the interaction of duration with time of day, day of week and month are strongly dependent on the
lifestyle and preferences of each user type. Depending on user type there was a disparity in trip duration during 
working hours. Also, the plots show a stable pattern of duration for subscribers across all levels of periodic variables
while customers had more variation in the relationship.


## Key Insights for Presentation

> For the presentation, I focus on just the influence of user type on individual rides. I start by introducing the
duration variable, followed by the pattern in user type distribution, then the relationship betwwen user type and duration.

> Afterwards, I introduce the interaction between duration and user type with each period variables.
To start, I use the plots of duration and day of week across user type. I'm only looking at
the boxplot here since it's the clearest example of how how user type affects duration across the week.
The other two period variables, time of day and month, are covered afterwards, using point plots and clustered bar charts.