

Online Databases
The database was sourced from http://insideairbnb.com/

You can find information on how he came to the conclusion on occpuancy rates here: http://insideairbnb.com/about.html#disclaimers

Actual occupancy data was scraped from AirBnB Calender's API

In summary, how current occupancy rates are calculated
A Review Rate of 50% is used to convert reviews to estimated bookings.

An average length of stay is configured for each city, and this, multiplied by the estimated bookings for each listing over a period gives the occupancy rate

The occupancy rate was capped at 70% - a relatively high, but reasonable number for a highly occupied "hotel".

Number of nights booked or available per year for the high availability and frequently rented metrics and filters were generally aligned with a city's short term rental laws designed to protect residential housing.

Basically to get average monthly income levels for an AirBnb, they take amount of reviews per month *2, multiple buy the average length of air bnb stay (4.5-5.2) and then multiply by the price per night.

They also say the max occupancy can only be 70% for the year, this give the variance in the air bnb length stay

My hypothesis's
Basing occupancy rates on yearly average of reviews I believe is a limited method. My hypothesis is to scrap data on listing that you can confidently says (as much as possible) are either booked or available. I believe you can find these listing be filtering by hosts that have 20 or more rental properties under their name, are willing to rent out the properties for more then 365 days in duration and offer "instant booking".

instant booking allows guests to book instantly with a AirBnB host, this mean their calender must be kept up to date or they will be penalized so it would be safe to assume that filtering by this and the features mentioned above, give you an accurate representation of a listing calender.

I believe booking like these can be confidently be seen to be operating as business with an aim to maximize occupancy