# Project 1: Standardized Test Analysis

### Overview

The SAT and ACT are standardized tests that many colleges and universities in the United States require for their admissions process. This score is used along with other materials such as grade point average (GPA) and essay responses to determine whether or not a potential student will be accepted to the university.

The SAT has two sections of the test: Evidence-Based Reading and Writing and Math ([*source*](https://www.princetonreview.com/college/sat-sections)). The ACT has 4 sections: English, Mathematics, Reading, and Science, with an additional optional writing section ([*source*](https://www.act.org/content/act/en/products-and-services/the-act/scores/understanding-your-scores.html)). They have different score ranges, which you can read more about on their websites or additional outside sources (a quick Google search will help you understand the scores for each test):
* [SAT](https://collegereadiness.collegeboard.org/sat)
* [ACT](https://www.act.org/content/act/en.html)

Standardized tests have long been a controversial topic for students, administrators, and legislators. Since the 1940's, an increasing number of colleges have been using scores from sudents' performances on tests like the SAT and the ACT as a measure for college readiness and aptitude ([*source*](https://www.minotdailynews.com/news/local-news/2017/04/a-brief-history-of-the-sat-and-act/)). Supporters of these tests argue that these scores can be used as an objective measure to determine college admittance. Opponents of these tests claim that these tests are not accurate measures of students potential or ability and serve as an inequitable barrier to entry.

### Problem Statement

**I have been hired by the College Board as part of a team to track statewide participation rates and recommend where and how money is best spent to improve SAT participation rates. With the data provided as well as some outside research, I hope to provide recommendations on improving participation rates in states by category.**

---

### Datasets

#### Provided Data used

Here are the six datasets used out of the 10 datasets provided. Additional data has also been used.

* [`act_2017.csv`](./data/act_2017.csv): 2017 ACT Scores by State ([source](https://blog.prepscholar.com/act-scores-by-state-averages-highs-and-lows))
* [`act_2018.csv`](./data/act_2018.csv): 2018 ACT Scores by State ([source](https://blog.prepscholar.com/act-scores-by-state-averages-highs-and-lows))
* [`act_2019.csv`](./data/act_2019.csv): 2019 ACT Scores by State ([source](https://blog.prepscholar.com/act-scores-by-state-averages-highs-and-lows))
* [`sat_2017.csv`](./data/sat_2017.csv): 2017 SAT Scores by State ([source](https://blog.collegevine.com/here-are-the-average-sat-scores-by-state/))
* [`sat_2018.csv`](./data/sat_2018.csv): 2018 SAT Scores by State ([source](https://blog.collegevine.com/here-are-the-average-sat-scores-by-state/))
* [`sat_2019.csv`](./data/sat_2019.csv): 2019 SAT Scores by State ([source](https://blog.prepscholar.com/average-sat-scores-by-state-most-recent))

#### Additional Data
* [`external_state_mandatory_testing.csv`](./data/external_state_mandatory_testing): States and the mandatory or optional testing they carry out.
([source1](https://blog.prepscholar.com/which-states-require-the-sat))
([source2](https://blog.prepscholar.com/which-states-require-the-act-full-list-and-advice))
([source3](https://www.edweek.org/teaching-learning/what-tests-does-each-state-require))

---

### Data Dictionary

1. merged_act_final file Data Dictionary:

|Feature|Type|Dataset|Description|Empty Cells|
|---|---|---|---|---|
|state|object|merged_act_final|String names of all the states for participants of the tests|0 Cells Empty|
|participation_act_17|float|merged_act_final|Represents the participation rate for 2017 in decimals for each state. (e.g. Colorado - 0.11)|1 Cell Empty|
|participation_act_18|float|merged_act_final|Represents the participation rate for 2018 in decimals for each state. (e.g. Colorado - 0.11)|2 Cells Empty|
|participation_act_19|float|merged_act_final|Represents the participation rate for 2019 in decimals for each state. (e.g. Colorado - 0.11)|1 Cell Empty|
|english_17|float|merged_act_final|Mean score of the participants in English for ACT for the year of 2017|1 Cell Empty|
|math_act_17|float|merged_act_final|Mean score of the participants in Math for ACT for the year of 2017|1 Cell Empty|
|reading_17|float|merged_act_final|Mean score of the participants in Reading for ACT for the year of 2017|1 Cell Empty|
|science_17|float|merged_act_final|Mean score of the participants in Science for ACT for the year of 2017|1 Cell Empty|
|composite_17|float|merged_act_final|Mean composite score of the participants for ACT for the year of 2017|1 Cell Empty|
|composite_18|float|merged_act_final|Mean composite score of the participants for ACT for the year of 2018|2 Cells Empty|
|composite_19|float|merged_act_final|Mean composite score of the participants for ACT for the year of 2019|1 Cell Empty|

2. merged_sat_final file Data Dictionary

|Feature|Type|Dataset|Description|Empty Cells|
|---|---|---|---|---|
|state|object|merged_sat_final|String names of all the states for participants of the tests|0 Cells Empty|
|participation_sat_17|float|merged_sat_final|Represents the participation rate for 2017 in decimals for each state. (e.g. Colorado - 0.11)|0 Cells Empty|
|participation_sat_18|float|merged_sat_final|Represents the participation rate for 2018 in decimals for each state. (e.g. Colorado - 0.11)|0 Cells Empty|
|participation_sat_19|float|merged_sat_final|Represents the participation rate for 2019 in decimals for each state. (e.g. Colorado - 0.11)|0 Cells Empty|
|ebrw_17|float|merged_sat_final|Mean score of the participants in Evidence-Based Reading & Writing for ACT for the year of 2017|0 Cells Empty|
|math_sat_17|float|merged_sat_final|Mean score of the participants in Math for SAT for the year of 2017|0 Cells Empty|
|total_17|float|merged_sat_final|Mean total score of the participants for SAT for the year of 2017|0 Cells Empty|
|ebrw_18|float|merged_sat_final|Mean score of the participants in Evidence-Based Reading & Writing for ACT for the year of 2018|0 Cells Empty|
|math_18|float|merged_sat_final|Mean composite score of the participants for SAT for the year of 2018|0 Cells Empty|
|total_18|float|merged_sat_final|Mean total score of the participants for SAT for the year of 2018|0 Cells Empty|
|ebrw_19|float|merged_sat_final|Mean score of the participants in Evidence-Based Reading & Writing for SAT for the year of 2019|0 Cells Empty|
|math_19|float|merged_sat_final|Mean composite score of the participants for SAT for the year of 2019|0 Cells Empty|
|total_19|float|merged_sat_final|Mean total score of the participants for SAT for the year of 2019|0 Cells Empty|

3. merged_all_final file Data Dictionary

|Feature|Type|Dataset|Description|Empty Cells|
|---|---|---|---|---|
|state|object|merged_sat_final|String names of all the states for participants of the tests|0 Cells Empty|
|participation_act_17|float|merged_all_final|Represents the participation rate for 2017 in decimals for each state. (e.g. Colorado - 0.11)|1 Cell Empty|
|participation_act_18|float|merged_all_final|Represents the participation rate for 2018 in decimals for each state. (e.g. Colorado - 0.11)|2 Cells Empty|
|participation_act_19|float|merged_all_final|Represents the participation rate for 2019 in decimals for each state. (e.g. Colorado - 0.11)|1 Cell Empty|
|participation_sat_17|float|merged_all_final|Represents the participation rate for 2017 in decimals for each state. (e.g. Colorado - 0.11)|2 Cells Empty|
|participation_sat_18|float|merged_all_final|Represents the participation rate for 2018 in decimals for each state. (e.g. Colorado - 0.11)|2 Cells Empty|
|participation_sat_19|float|merged_all_final|Represents the participation rate for 2019 in decimals for each state. (e.g. Colorado - 0.11)|2 Cells Empty|
|english_17|float|merged_all_final|Mean score of the participants in English for ACT for the year of 2017|1 Cell Empty|
|math_act_17|float|merged_all_final|Mean score of the participants in Math for ACT for the year of 2017|1 Cell Empty|
|reading_17|float|merged_all_final|Mean score of the participants in Reading for ACT for the year of 2017|1 Cell Empty|
|science_17|float|merged_all_final|Mean score of the participants in Science for ACT for the year of 2017|1 Cell Empty|
|composite_17|float|merged_all_final|Mean composite score of the participants for ACT for the year of 2017|1 Cell Empty|
|composite_18|float|merged_all_final|Mean composite score of the participants for ACT for the year of 2018|2 Cells Empty|
|composite_19|float|merged_all_final|Mean composite score of the participants for ACT for the year of 2019|1 Cell Empty|
|ebrw_17|float|merged_all_final|Mean score of the participants in Evidence-Based Reading & Writing for ACT for the year of 2017|2 Cells Empty|
|math_sat_17|float|merged_all_final|Mean score of the participants in Math for SAT for the year of 2017|2 Cells Empty|
|total_17|float|merged_all_final|Mean total score of the participants for SAT for the year of 2017|2 Cells Empty|
|ebrw_18|float|merged_all_final|Mean score of the participants in Evidence-Based Reading & Writing for ACT for the year of 2018|2 Cells Empty|
|math_18|float|merged_all_final|Mean composite score of the participants for SAT for the year of 2018|2 Cells Empty|
|total_18|float|merged_all_final|Mean total score of the participants for SAT for the year of 2018|2 Cells Empty|
|ebrw_19|float|merged_all_final|Mean score of the participants in Evidence-Based Reading & Writing for SAT for the year of 2019|2 Cells Empty|
|math_19|float|merged_all_final|Mean composite score of the participants for SAT for the year of 2019|2 Cells Empty|
|total_19|float|merged_all_final|Mean total score of the participants for SAT for the year of 2019|2 Cells Empty|
|mandatory_17|object|merged_all_final|String categories of whether the state has mandatory testing for ACT or SAT. This list is active as of 2017 If the state does not have mandatory testing, then it is indicated as optional.|2 Cells Empty|

---

### Brief Summary of Analysis

#### Cleaning:
1. First of all, I explored the data files provided. It was clear that there were some issues with the files. The data types were not right which was the first thing that I fixed. This required cleaning some of the columns and changing the data type. I renamed the columns and began the cleaning phase. 
2. After cleaning and changing the data types, of the participation columns. Two of the rows in the SAT_2019 file had no participation rates. So it was decided to drop those rows as without the participation rate, whether it was high or low, it would have to be omitted from the analysis anyway.
3. After this, I merged the files before checking for the maximum and minimum score values.
4. The reason for checking the maximum and minimum values is that there cannot be negative participation rates or rates more than 1. Same for the scores, there were maximum and minimum scores which were checked. Upon checking this, I found that the math minimum score from the SAT_2017 file was invalid, and there was also a suspiciously low score found in the ACT_2017 file under the science column. 
    - For both of them, the score was changed as there were strong indicators that the score had just been input incorrectly.
5. Lastly, from the additional file I dropped all columns that were unnecessary.

#### EDA:
1. I looked at summary statistics to get a quick feel for the data.
2. Next I looked at the highs, lows, and the 50% mark for the participation rates across all three years for both the ACT and SAT. There were some interesting insights uncovered.
3. We also looked at the maximum and minimum total/composite scores obtained by the participants of both tests. 

#### Visualization:
Armed with some knowledge about the data from the EDA, I dove into the visualizations.
1. First, I started with looking at Seaborn's heatmap to identify correlations and guide other plots.
2. Next, I Plotted histograms for every column to see if there was any insight the distributions could shed on the data.
3. After that I created boxplots and scatterplots and that is where I started to see a clearer picture. 
4. With all of these visualizations and the EDA, I had managed to pull out some insights from the data that allowed me to make some reccommendations to the problem statement above.

---

### Conclusions and Recommendations:

### Key takeaways from the data:
1. The ACT and SAT participation rates are inversely related. Those states that have 100% ACT participation, are those that have state mandated ACT testing. 
    
    **Recommendation**: 
    - Target the state level selection committees and pitch them the new and improved SAT to use over the ACT or any other test.
    - The states that fall into this category are: Mississippi, Kentucky, Wisconsin, Utah, Tennessee, Ohio, Nebraska, Montana, Alabama, Louisiana, Wyoming, Arkansas, North Dakota, Minnesota, Missouri, South Dakota, Kansas, Iowa, New Mexico.
    

2. There are a few states with more than 50% participation rates for both tests. These states are the states that do not mandate 1 or the other test, rather it is optional where the students choose.
    
    **Recommendation**: 
    - Here we would suggest a two pronged approach. 
    - First, market to the students why they should choose the SAT over the ACT and the benefits the new and improved SAT provides in terms of giving them a more comprehensive score based on their aptitiude. 
    - Second, approach the state as well (at the same time if possible), starting with those where the SAT participation rates are more than the ACT participation rates. The argument here is that the students already have a preference, why not make this a state mandate, (like many other states have done), which will allow the student foresight on which test they will need to do. This means that they can likely start their prep much earlier, instead of rushing in the three months leading up to the test.
        - The states falling into this category are: Georgia, South Carolina, Hawaii, North Carolina
    

3. The test participation rates and scores are inversely proportional, meaning as participation rates go up, the mean scores per state will decrease.
    
    **General Recommendation**: 
    - As the SAT participation rates go up, we would have to deploy additional resources to states where they have contracted with the college board to use the SAT statewide. The purpose of these resources would be to help the schools and students understand where they can improve the SAT and how they can get a higher score.
    - Maintaining or improving the mean state score will potentially 'future-proof' the adoption of the SAT as we would have shown that even with higher participation rates, the college board is able to deploy enough resources to the states that have contracted with us. This may prompt other states to enter into a contract as well.
