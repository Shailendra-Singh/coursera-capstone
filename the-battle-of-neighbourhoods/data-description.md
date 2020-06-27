---
layout: page
title: "The Battle of Neighborhoods"
description: "IBM Data Science Professional Certificate - Applied Data Science Capstone"
permalink: the-battle-of-neighborhoods/data-description
show_home: "true"
show_project_home: "true"
is_product_page: "true"
project_url: /coursera-capstone/the-battle-of-neighborhoods
repository_url: "https://github.com/Shailendra-Singh/coursera-capstone/tree/master/Projects/Battle%20of%20Neighbourhoods"
---
`20th June, 2020` **·** `1 min read`

## B. Data Description

The dataset which I'm using in this project can be acquired from [here](https://sites.google.com/site/yangdingqi/home/foursquare-dataset). This dataset is originally used for studying the spatial-temporal regularity of user activity in LBSNs **[1]**.

This dataset includes long-term (about 10 months) check-in data in New York city and Tokyo collected from *Foursquare* from 12 April 2012 to 16 February 2013 **[2]**.

It contains two files (NYC and TKY) in tsv format. Each file contains 8 columns, which are:
1. User ID (anonymized)
2. Venue ID (Foursquare)
3. Venue category ID (Foursquare)
4. Venue category name (Fousquare)
5. Latitude
6. Longitude
7. Timezone offset in minutes (The offset in minutes between when this check-in occurred and the same time in UTC)
8. UTC time

NYC DataFrame e.g.:

|userId|venueId|venueCategoryId|venueCategory|latitude|longitude|timezoneOffset|checkInUtcTimestamp|
|:----:|:-----:|:-------------:|:-----------:|:------:|:-------:|:------------:|:----------:|
|470|49bbd6c0f964a520f4531fe3|4bf58dd8d48988d127951735|Arts & Crafts Store|40.719810|-74.002581|-240|Tue Apr 03 18:00:09 +0000 2012|


There are around 2.27m check-ins in New York City and 5.37m check-ins in Tokyo City. In above columns, the semantic meaning of a check-in can be found from 'Venue Category Name' (from Foursquare - Endpoint: '/venues/categories' ) column.

### References 
--------------

##### **[1]** _Dingqi Yang, Daqing Zhang, Vincent W. Zheng, Zhiyong Yu. Modeling User Activity Preference by Leveraging User Spatial Temporal Characteristics in LBSNs. IEEE Trans. on Systems, Man, and Cybernetics: Systems, (TSMC), 45(1), 129-142, 2015._ [[PDF]](http://www.google.com/url?q=http%3A%2F%2Fwww-public.it-sudparis.eu%2F~zhang_da%2Fpub%2FTSMC_YANG_2014.pdf&sa=D&sntz=1&usg=AFQjCNGSbghKxMGgmh6S1Hd-uz3SIkbLqQ)

##### **[2]** _Foursquare_ [API](https://developer.foursquare.com/)