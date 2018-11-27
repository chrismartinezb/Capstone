# Google Store Customer Predictions

# Install

This project requires **Python 3.6** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)
- [seaborn](https://seaborn.pydata.org/)
- [bayes_opt](https://github.com/thuijskens/bayesian-optimization)
- [xgboost](https://xgboost.readthedocs.io/en/latest/)

## Data

You can download all the datasets used in this project in the following links:

-[Raw Data](https://www.dropbox.com/s/o8aqviril0xqrvn/data.zip?dl=0)

-[Parsed Data](https://www.dropbox.com/s/a40y2yiknobs6ct/Data-flattened.zip?dl=0 )

We have a dataset of approximately 90 thousand rows , each corresponding to a single visit to the store[2]. Each row has the next columns:

1)fullVisitorId- A unique identifier for each user of the Google Merchandise Store.

2)channelGrouping - The channel via which the user came to the Store.

3)date - The date on which the user visited the Store.

4)device - The specifications for the device used to access the Store.

5)geoNetwork - This section contains information about the geography of the user.

6)socialEngagementType - Engagement type, either "Socially Engaged" or "Not Socially Engaged".

7)totals - This section contains aggregate values across the session.

8)trafficSource - This section contains information about the Traffic Source from which the session originated.

9)visitId - An identifier for this session. This is part of the value usually stored as the _utmb cookie. This is only unique to the user. For a completely unique ID, you should use a combination of fullVisitorId and visitId.

10)vsitNumber - The session number for this user. If this is the first session, then this is set to 1.

11)visitStartTime - The timestamp (expressed as POSIX time).

12)hits - This row and nested fields are populated for any and all types of hits. Provides a record of all page visits.

13)customDimensions - This section contains any user-level or session-level custom dimensions that are set for a session. This is a repeated field and has an entry for each dimension that is set.

14)totals - This set of columns mostly includes high-level aggregate data.


