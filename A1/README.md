#HCDE410
Files for HCDE410 - Assignment A1

Adapted from # cdsw-2020 https://wiki.communitydata.science/Seattle_open_data

```
# A1 — Working with Open Data

**Dataset:** Burke-Gilman Trail counter north of NE 70th St
**Source:** https://data.seattle.gov/Transportation/.../2z5v-ecg8  (pulled 2026-10-12)
**License / terms of use: This is a public data set 

## Questions I asked
- Q1. When is the trail busiest, and when is it quietest?
 
- Q2. Do cyclists and pedestrians use the trail at different times of day?
- Q3. Commuting or recreation?  Is there evidence people use the Burke-Gilman to commute, not just for fun?
- Q4. Direction and flow. The counter records north vs. south separately. Are mornings mostly one direction and evenings the other? What would that tell you about who's using the trail and where they're heading?


## How to re-run
Open `A1.ipynb` and run all cells (needs `requests`, `pandas`, `matplotlib`).
Find the total number of bikes and pedestrians by adding them together for each hour. Then print the data and manually find the maximum and minimum amount of activity to find out when the trail is the busiest and quietest.

```