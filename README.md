# Is-Fandango-Still-Inflating-Ratings-

In October 2015, Walt Hickey from FiveThirtyEight published a popular article where he presented strong evidence which suggest that Fandango's movie rating system was biased and dishonest.

Fandango displays a 5-star rating system on their website, where the minimum rating is 0 stars and the maximum is 5 stars. At that time, the real Fandango rating (which was different than its displayed star rating) was in the HTML for the page. Hickey compared the real and displayed ratings and found egregious rounding issues that led to the discrepancy between the number of stars displayed to users and the actual rating. He was able to find that:

The actual rating was almost always rounded up to the nearest half-star. For instance, a 4.1 movie would be rounded off to 4.5 stars, not to 4 stars, as you may expect.
In the case of 8% of the ratings analyzed, the rounding up was done to the nearest whole star. For instance, a 4.5 rating would be rounded off to 5 stars.
For one movie rating, the rounding off was completely bizarre: from a rating of 4 in the HTML of the page to a displayed rating of 5 stars.
It's been nearly 5 years since the FiveThirtyEight piece was published, and we want to know: is Fandango still up to the same shenanigans, or did they fix what they claimed was a bug in their system? The actual rating values are no longer displayed in the pages' HTML, so we don't immediately know how the scores are rounded. We will investigate if there has been any change in what was five years ago a problematic and dishonest rating system.

In this project, we'll analyze more recent movie ratings data to determine whether there has been any change in Fandango's rating system after Hickey's analysis.
