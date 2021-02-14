## Fuzzy Geocoding

When analyzing social media data we, often want to add a geographic element to the activity. 
This isn't always so easy due to data availability and user practices with location disclosure. 
Here I run over some preliminary results from my first experience with attempting fuzzy-string geocoding 
on Twitter user provided location strings. 


There are a couple ways to go about geocoding for Twitter. 
The easiest case is obviously when the user enables geolocation and precise(ish) coordinates are available for the activity.
This has its limitations, especially in more recent years (~2015+) where changes to Twitter defaults have left very
few accounts with geolocation enabled (there are also concerns about the types of accounts likely to enable this feature).
At one point I found less than 1% of tweets in our random 10% sample had precise geolocation information available. 

The other approach that I've seen some colleagues explore involves fuzzy string matching and geocoding. 
