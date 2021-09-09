### DFGVancouver_Brightside2021_in_the_works

#### Datathon with Data For Good Vancouver, in cooperation with Brightside

Analysis of Brightside housing data.  

#### 1.  rodriguez_2021

Datathon day.  Processed 2021 crime data per neighbourhood.  Manually linked neighbourhood and postal code.  Merged with Amenities dataset.  Analyzed buildings' neighbourhood 2021 crime rate.

#### 2.  survey2020

2020 survey variables trimming of variables.

#### 3.  survey2020 clean

2020 survey trimmed variables, null values filled.  Ready for EDA.

#### 4.  survey'20 EDA 9_5

Using cleaned 2020, removed mod-high correlated variables,checked plots of location vs others - checked survey questions and answer values.  Initially did some location-based plotting, however, might need to resort back to df.hist due to inapplicability of taking the mean (values not really ordinal).

-> Task: convert 'prefer not to answer' asnwers to NaN, recheck missing val distribution.

#### 5.  DFG_B_df10

Cleaned Survey 2020 dataset.  Removed irrelevant variables, replaced 'prefer not to answer' values with Nan, removed variables with >10% missing, removed mod-highly correlated variables.

#### 6.  survey'20_EDA_9_8_1pm

Using df10, fast EDA using hist.
categorical = location, gender, rln_status, work_paid, work_vol, bside_pre
binary = household, walk_aid, imm_status, bside_pre_muni,
ordinal = nbr_relation, food_worry, apprch_bside, hlth_happy, chat_often, rlns_safe, age, bside_dur

Findings:
Most tenants are Canadian-born, aged >55, female, single and living by themselves.

Most are retirees, not doing volunteer work.

Majority were not worried about food. They had acceptable neighbourly social interactions and generally felt content and safe.

Most tenants were previously renting from private companies in Vancouver and are now long-term Brightside clients who think that Brightside is approachable.

Limitations:
Findings might be skewed by representation bias.

Task:  Get means, merge with Assets dataset.

#### 7.  means

Created dataset indexed by locations, populated by means of the ordinal and binary variables.

For merging with Assets.

#### 8 and 9.  crime.csv and crime.ipynb

Created 2020 crime dataset, for merging with Assets and Means.

#### 10 and 11.  means_ass_crime.csv and .ipynb

Merged Survey 2020 means, Assets and 2020 neighbourhood crimes.
