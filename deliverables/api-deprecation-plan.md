A model for deprecating a live API:  

* Analyze the API analytics to understand how many people use the API, how much, and what for.  
* Weigh whether the API can be deprecated by letting it remain live but with the API documentation updated to clearly indicate that it is no longer supported and the current users emailed to notify them of this change.  This will allow soft landings and departures on their own timetables.  
* If the decision is made to turn off the API, plan out a communications plan and allow yourself time to implement it appropriately.  A rushed or unexpected API turnoff will harm developer goodwill and their willingness to use your products in the future.  
* Update the API documentation to feature a *very* prominent message that announces the deprecation and it's planned timing and points to alternatives if they exist.  
* Consider removing the API key signup form from the API documentation.  
* Email current users of the API with news of the deprecation, including the reasoning and timetable, and points to alternatives if they exist.  
* I recommend at least 3-4 weeks of lead time for these announcements, preferably more.  If you don't allow this much time, there's a real chance that the developer doesn't have time to explore alternatives and calmly phase out their use of the API before it's deprecated.  Turning off the API with little warning is a very real form of the pain that we would cause them if we turned off the API with no warning.  
