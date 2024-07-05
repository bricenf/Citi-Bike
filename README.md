# Citi-Bike Data Analysis

An unpublished version uses climate/environment raster data to overlay Citi-Bike usage during particular weather conditions such as heat/rain/etc. It could be used to understand how New Yorkers use Citi-Bikes during particular weather occurances. Therefore, we could integrate different micro-transit or mass-transit solutions in robust ways to adapt to weather. Additionally, it uses Open-Street-Map data to find openly sourced public resources (such as libraries, parks, etc.) and private resources (hotels, food options, etc.) to see where Citi-Bikes are most active. 

Data uses Open Source Maps and Citi-Bike data directly from Lyft. 

This version: Takes data from Citi-Bike and overlays the geocordinates to Open-Street-Map data. 
  (1) Creates a sub-data frame, utilizing data from the initial information provided. For example, past data-sets provided duration of each trip, but Lyft stoppped adding that data. Instead, you can create the duration by a new column that subtracts the end time from the start time. Also, you could calculate the average speed of a Citi-Bike, taking the distance and dividing it by the duration. Do New Yorkers follow Citi-Bike rules or street rules? Some micro-transit solutions cap off speed in high dense or special areas, is that something we should implement?
  (2) Creates a hot map of where Citi-Bikes are most in use
  (3) Takes each trip, and loops it through Open-Street-Maps to find the optimal route a biker would take. This assumes that each biker either (a) knows the city as well as a driver would, which streets are one way and what's optimal routes, or (b) uses a GPS
  (4) Finds which streets are most used by Citi-Bikes, this could be used to inform DOT or city agencies on which areas should be priotized for bike improvements or ensured safe routes as they are most used
  (5) Tests the seasonality of Citi-Bike usage across months. Does Citi-Bike usage spike in the summer vs. winter? If so, could we optimize how many Citi-Bikes are in the city? Is there a need for Citi-Bikes to take up street space when they are not in demand?
  (6) Looks at the distribution of Citi-Bikes across months. At what duration does the average biker take? Are these systems designed for New Yorkers? What is the average duration a biker takes and does that duration change month to month? If it's hot, or cold, is a biker taking the same duration? How consistent are they to biking for the same time or distance?
