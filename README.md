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
