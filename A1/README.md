#HCDE410
Files for HCDE410 - Assignment A1

Adapted from # cdsw-2020 https://wiki.communitydata.science/Seattle_open_data

```
# A1 — Working with Open Data

**Dataset:** Burke-Gilman Trail counter north of NE 70th St
**Source:** https://data.seattle.gov/Transportation/.../2z5v-ecg8  (pulled 2026-10-12)
**License / terms of use: This is a public data set 

## Questions I asked

- Q1. When is the trail busiest, and when is it quietest? Decide what busy means to you first — a single hour? a stretch of the day? bikes and peds together, or separately? — and say why you chose that.

   For this question, my thought process for when the trail was the busiest was when both cyclist and pedestrians were on the trail on the time scale of a single hour.

- Q2. Do cyclists and pedestrians use the trail at different times of day? Compare their hourly patterns. If they differ, what might explain it?

    For this question I thought about comparing the amount of pedestrians and cyclist on an hourly bases and seeing when is there a maximum and minimum usage of the trail from pedestrians vs from cyclist?


- Q3. Commuting or recreation? Is there evidence people use the Burke-Gilman to commute, not just for fun? Compare weekdays vs. weekends (we made a weekday column for you), and maybe morning vs. evening. Define what a "commuting pattern" would look like in the data, then say whether you see it.

    For this question I thought about creating a list of pedestrians and cyclist combined on a daily bases to compare their commuting pattern to see if there is a increase in usage of the trail on the weekends that counts as recreation. I also looked at total amount of bikes and pedestrians combined for each hour to see if there was more usage of the trail in the morning or evenings.  I counted mornings as 12AM - 11AM and evenings as 5PM-12PM. 


- Q4. Direction and flow. The counter records north vs. south separately. Are mornings mostly one direction and evenings the other? What would that tell you about who's using the trail and where they're heading?

    For this question I wanted to combine the bikes and pedestrian uses for both the north and south counters in order to see the difference between them. I then thought about how many combined bikes and pedestrians were spotted for each hour for each direction. I spotted a pattern of more usage at 8Am going north and more usage at 5PM going south, this could indicate that people are traveling to work up north at 8AM and back home south at 5PM.


## How to re-run
Open `A1.ipynb` and run all cells (needs `requests`, `pandas`, `matplotlib`).

Q1.
Find the total number of bikes and pedestrians by adding them together for each hour. Then print the data and manually find the maximum and minimum amount of activity to find out when the trail is the busiest and quietest.

Q2.
Print a list of the bikes and pedestrians on an hourly bases on 2 different columns. Manually inspect when the maximum and minimum is for both bikes and pedestrians in order to see if there is a difference in hours.

Q3.
Group the number of bikes and pedestrians by days. Then add up the bikes and pedestrians together for each day and print that out as a list. Manually inspect it to see if there is a difference in number on the weekends to see if the trail is being used recreationally. To see if there is a difference between mornings and evenings, use the same list from earlier and check mornings as 12AM - 11AM and evenings as 5PM-12PM to see if there is a difference in activities. 

Q4.
Combine the number of bikes and pedestrians for the north and south separately then group it by hours to create a list with 3 separate columns of time, north and south. Print this list out and manually find the maximum from each list to see when the direction is used the most. 

```