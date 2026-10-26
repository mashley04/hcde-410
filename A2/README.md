#HCDE410
Files for HCDE410 - Assignment A2

```
# A2 — Exploring sources of bias in data

**Dataset:** Toxicity dataset, Aggression dataset, Personal Attacks dataset

**Source:** https://figshare.com/projects/Wikipedia_Talk/16731 (pulled 2026-10-24)

**Publisher** Ellery Wulczyn

**License:( https://creativecommons.org/publicdomain/zero/1.0/) The person who associated a work with this deed has dedicated the work to the public domain by waiving all of his or her rights to the work worldwide under copyright law, including all related and neighboring rights, to the extent allowed by law.
You can copy, modify, distribute and perform the work, even for commercial purposes, all without asking permission.

**Terms of use: (https://figshare.com/terms) Without prejudice to any Published Content Licence or Contract, the Service is provided only for your personal, non-commercial research purposes, at all times subject to these Terms. You shall not otherwise use any part of the Service without the prior and express written agreement of Figshare.

## Questions I asked:

Question 1: What is the gender distribution of these workers?¶

Question 2: What is the distribution of the workers by first language?

Question 3: What is the distribution of these workers by age group?

Question 4: what is the distribution of these workers by education level?

Question 5: Analyze all_annotators in Sheets or Jupyter: Do any of the fields in this dataset have missing data? If so, which fields, and what % of the rows contain missing values?

Question 6: Build a version of the all_annotators dataset without removing duplicates, then re-run the summary statistics from questions 1-4. How have these summary statistics changed?

Question 7: In general, how do the demographics of these workers compare to those of English-speaking internet users overall? Why would it matter if the worker demographics don't match the demographics of the intended end users of the Perspective API?¶

Question 8: Given what you now know about the Wikipedia Talk Corpus, what issues might arise if it was used to train a machine learning-driven "hostile speech detector" that could be used on any website or social media platform?

Question 13: Pick 2-3 examples of comments where you disagreed with the labeller about the toxicity of a comment. Why did you disagree? Why do you think that the labeller might have labelled these comments the way they did?

Question 14: Pick 2-3 examples of comments where you don't understand what the commenter was saying, and therefore had a hard time classifying as toxic or non-toxic. What additional context or information would you need in order to be confident in your judgement about the toxicity of this comment?

Question 15: Read through the instructions and labelling options given to the crowdworkers. How could the way these instructions were written have made it difficult for crowdworkers to accurately label comments as toxic or non-toxic? If you were going to run a labelling campaign like this one yourself, how would you change these instructions or labelling options to help the crowdworkers make more accurate or consistent judgements about toxicity?

Question 16: Based on your findings from questions 13-15, how might this dataset present a biased view of "toxicity"? How would you expect such biases to impact how the Perspective API performs as a general-purpose hostile speech detector? 

## How to re-run:
 
Questions 1-4:

In order to determine the demographic of the workers in the dataset, we first need to create bar charts and tables by running panda to examine the statistics.

Input: all_annotators file. Replace every missing value (white spaces) with unknown.

Output:

(Bar charts) 
Sorted from highest to lowest per demographic label. Each bar chart has a different demographic (age, gender, language, education)
x-axis: demographic labels
y-axis: number of annotators. 

(Summary Table)
Count and percentage of the demographic rounded to 2 decimals.


Question 5:

Use the original all_annotators dataset to create a table showing how many white spaces/ missing data is in each category for demographics (age, gender, language, education). Because age_group is the only category with missing data, we can use that number and divide it by the total about of annotators there are and multiply it by 100 to find the percentage of rows that contain missing values.

Input: all_annotators dataset

Output: 
A table displaying:
- The amount of missing data that is in each category. 
- The total number of annotators in the dataset.
- Percentage of rows that contain missing values rounded to 2 decimals.

Question 6:
Create 2 different dataset id's for attack and aggression in order to use the original data that was not de-duplicated in order to create a new csv that had the labels attack and aggression separated. 

Run the code to create bar charts and tables on the new csv dataset labeled all_annotators_dupe in order to find the summary statistic for each demographic.

Input: all_annotators dataset

Output: 
- Dataset that allows 3 labels (attack, aggrestion, toxicity)
- all_annotators_dupe (a dataset with all 3 label original datasets)
-Bar chart:
Sorted from highest to lowest per demographic label. Each bar chart has a different demographic (age, gender, language, education)
x-axis: demographic labels
y-axis: number of annotators. 
-Table: Count and percentage of the demographic rounded to 2 decimals.


Question 7:
This question did not use any code but I researched some of the demographics for internet users in general and compared it to the worker demographic in order to make my conclusions.

Question 8: 
This question did not have code and was opinions based.

Question 13: 
This question did not have code.
Opened toxicity_labelled_comments_3k_sample to examine 20 of each comment that were "toxic" (-1 or -2), "non-toxic" (1 or 2) and "neutral" (0) finding comments I disagreed on of the labelling. 


Question 14:
This question did not have code.
Opened toxicity_labelled_comments_3k_sample to examine 20 of each comment that were "toxic" (-1 or -2), "non-toxic" (1 or 2) and "neutral" (0) finding comments I did not understand or needed more information on before I would label the comment.

Question 15:
This question did not have code.
Read through the instructions and labelling options for workers and determine if there was anything that made labelling confusing and what I would change about it.

Question 16:
This question did not have code and was opinions based.

Limitations & Biases: One limitation this dataset has is on the age_group category the age ranges are overlapping (18-30, 30-45, etc), this can cause misrepresentation in the data analysis when looking at the distribution. Workers the age of 30 can qualify for 2 different age groups so putting them in one over the other skews the data.

```

