# Airbnb Occupancy Rates 

## *How many bookings can I hope to get in a month?* 

This is a a question asked by both homeowners looking to make additional income and governments curious about how short term letting affects prices in the hotel industry. 

As Airbnb doesn't make their substantial datasets public, we can't yet know the answer for certain, but there are workarounds. The most widely used option to gauge the occpuancy rates of a listing is through a review-based model. The model calculates expected occupancy from how many reviews a listing has recieved. This approach, however, is based on speculative reasoning.

My hypothesis is that this model can be improved by using modern predictive modelling techniques. 

The original Airbnb database was sourced from http://insideairbnb.com/.

You can find information on how Murray Cox came to the conclusion on occpuancy rates here: http://insideairbnb.com/about.html#disclaimers
Actual occupancy data was scraped from Airbnb's calender API.

## *How review-based occupancy rates are calculated:*
- A review rate of 50% is used to convert reviews to estimated bookings.

- An average length of stay is configured for each city, and this, multiplied by the estimated bookings for each listing over a period, gives the occupancy rate.

- The occupancy rate was capped at 70% - a relatively high, but reasonable number for a highly-occupied "hotel".

- Number of nights booked or available per year for the high availability and frequently-rented metrics and filters were generally aligned with a city's short term rental laws designed to protect residential housing.

- To get average monthly income levels for an Airbnb listing, they take amount of reviews per month *2, multiple buy the average length of an Airbnb stay (4.5-5.2) and then multiply by the price per night.

- They also say the max occupancy can only be 70% for the year.

## *My hypothesis:*
Basing occupancy rates on yearly average of reviews is, I believe, a limited method. My hypothesis is to scrape data on listings that you can confidently say are either booked or available. You can find these listings by:
- filtering by hosts that have 20+ rental properties under their name and
- are willing to rent out the properties for more then 365 days in duration and
- they offer "Instant Booking".

Instant Booking allows guests to book instantly with a Airbnb host. This means their calendar must be kept up to date or they'll be penalised by Airbnb. From this, it's logical to assume that filtering by this, and the features mentioned above, gives an accurate representation of a listing calender.

I believe bookings like these can confidently be seen to be operating as businesses with an aim to maximise occupancy.