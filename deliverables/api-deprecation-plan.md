A model for deprecating a live API:  

* Analyze the API analytics to understand how many people use the API, how much, and what for.  
* Weigh whether the API can be deprecated by letting it remain live but with the API documentation updated to clearly indicate that it is no longer supported and the current users emailed to notify them of this change.  This will allow soft landings and departures on their own timetables.  
* If the decision is made to turn off the API, plan out a communications plan and allow yourself time to implement it appropriately.  A rushed or unexpected API turnoff will harm developer goodwill and their willingness to use your products in the future.  
* Update the API documentation to feature a *very* prominent message that announces the deprecation, being sure to include its planned timing and points to alternatives if they exist.  
* Consider removing the API key signup form from the API documentation.  
* Email current users of the API (have made API calls within the past 1-2 month) with news of the deprecation, including the reasoning, a timetable, contact info for asking questions, and suggestions for alternative data sources if they exist.  
  * If there is an existing forum that would support this, it is worthwhile to give the developers a place where they can give feedback, ask questions, and support each other in the transition.  
* I recommend at least 3-4 weeks of lead time for these announcements, preferably much more.  If the API is well-established and popular, 3 months would be a better minimum.  If you don't allow this much time, there's a real chance that the developer doesn't have time to explore alternatives and calmly phase out their use of the API before it's deprecated.  Turning off the API with little warning is a very real form of the pain that we would cause them if we turned off the API with no warning.  

Optional: Even if the API has to be taken completely down, it can sometimes be nice to return a more helpful error page in it's place, if possible. So instead of returning some generic 404 Not Found or 502 Bad Gateway error (or the worst is really if the hostname completely disappears and the site doesn't respond at all), returning something like a 410 Gone page with a simple plain text response explaining that the API has been taken down (and point to any relevant links). This can be useful, since despite the best communication efforts ahead of time, you might still have users hitting the deprecated API when it goes completely down. By providing a more helpful error page, this can at least help a tiny bit (so the user isn't left scratching their head and wondering if the error responses are temporary).

_Note that the above is also relevant for deprecating API versions as well._
