# kickstarter-analysis
Unit 1 Excel work
# Kickstarting with Excel

## Overview of Project
    The Kickstarter data displays information about all sorts of proposed entertainment options, from plays to songs to technology.  This includes financial such as a cash goal regarding donations, the country, and great detail regarding each proposal.  Data good.  Bryan like.
### Purpose
    The client Louise has written a play Fever that is ready to present to the public.  In order to better understand the dates and costs for successful fundraising, it is required to examine the date.  In this sense, this includes launch dates (largely by month of the year) and funding goals.  This should address two questions of when to release it and ideal investment cost.
## Analysis and Challenges
    The analysis of this data is fairly straight forward.  It involves some minor conversions such as transforming a Unix time stamp into a legible date and year.  Some categories were also converted to subcategories and filters were applied to better organize the data during viewing.  On my end, the most challenging part was working with the COUNTIFS function where 0 < x < 100 would have to be split into two completely spearate statements.  This is not as intuitive as a lot of other functions.
### Analysis of Outcomes Based on Launch Date
    The most important trend to view is that there is a large spike in success rates in the months of May and June.  This is opposite with the months of November and December where success rates are significantly lower.  The rate of cancellation is generally low but shows a slight increase in January possibly as a follow-up affect to the Nov./Dec. decrease.  The failed category is arguably linear although there is a slight decrease from Nov. to Mar.  There does not appear to be any other relationship between the three categories.
### Analysis of Outcomes Based on Goals
    When examining successful versus failed, it is interesting to observe that they are inversy proportional with respect to funding.  The success rate is terminated after the range of $40k to $45k.  In the lower range (~5000 to 24999), one observes an almost 50:50 chance for a play to succeed or fail.
### Challenges and Difficulties Encountered
    Largely, it took some effort to produce the correct criteria with COUNTIFS with Outcomes Based on Goals.  Being a more precise formula, it therefore requires more effort to manually alter each criteria moving down the table.  Unix code is also not dealt with very smoothly with excel and required true knowledge of a particular calculation.
## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
With respect to Launch date, one should consider a release in late spring, early summer when more shows are accepted by the public.  This is opposite to Nov/Dec which is very low.  There is relatively little change time-wise for failure shows.

- What can you conclude about the Outcomes based on Goals?
With respect to funding, the success options are between 5000 and 14999 or 35000 and 44999.

- What are some limitations of this dataset?
The dataset is relatively simple, showing funding, dates, and a brief description.  This limits the analysis towards simple conclusions.  The countries explored are also relatively few and have potential to skewer the data towards the USA.  Information regarding actors, play-type or age attracted can further add to the understanding.

- What are some other possible tables and/or graphs that we could create?
Proper text analysis may be able to pull out keywords in the "blurb" column that would give insights towards common factors.  For specific launching interest, one may consider plotting deadline versis launched_at to gain an understanding of wait time.  The number of backers the the ammount pledged inside each funding range (i.e. 5000 to 14999) may also provide some interesting insights.