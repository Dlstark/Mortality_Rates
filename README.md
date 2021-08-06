
# **Life as we know.**

 ## **Introduction:** 
What is one thing that everybody has, yet everyone is different? 
Life… Life is the single most important thing a person can have. That is 
why it is so crucial that we sustain and preserve it. How has life been 
for us since 1980 up into 2014? Here we will take a deep dive using big 
data into life expectancy and mortality rates using a few different 
variables. Breaking down every single state by individual county we will 
determine the male and female life expectancy and mortality rate using ages 
0 through 85. My main goal on this journey will be to see how each 
county/state has progressed or regressed over the 34-year span. 


## **Motivation/why should you care:**
The word “life” has always felt so strange to me. Is it just a number with 
age, a long road of A to B, or what you make of it from beginning to end? 
There is so much that plays a factor in it, so I really wanted to dig deep
and look at the life expectancies and mortality rates. What I found was a 
large data set breaking those variables down county by county, state by 
state to see how rates have increased or decreased. I am excited to
breakdown the male and female mortality risks state by state to better
understand how America has progressed from the years 1980 through 2014.

## **Tools Used:**
Excel, Python(Pandas), and Tableau


## **Challenges:** 
- The first challenge I across was how i wanted to break down my data and my 
plan of attack for EDA. I had 6 worksheets in a workbook si wanted to break 
thos down to 6 seperate CSV files to make digesting the data easier to
accomplish.
- After they were CSVs i had to come up with a plan of attack on how to make
the columns and rows line up. Some CSVs had the county and state in the 
same cell, while others were split between two cells. So, I had to come 
up with the formula in excel in order to split the shared cells up to
match the other CSV files.
- Then I had to worry about counties whose name was two words. My initial
 formula in excel was based off of a space so then I had to readjust that
 in order to pick up both words that made up the county
- Next I pulled all of the CSVs into Python(Pandas) where the majority
 of my deep cleaning and shaping came from.
- Every cell had three values in it. There was a male average, a female
average, and their combined average. So, I had to figure out a code 
that would simultaneously split those three values into three different
cells in a new column, rename those new columns, and take off any 
quotations or parentheses that were attached to the value. This would 
also drop the original cell that the three values were originally in.
- After I was able to split those values and put them in a male, female,
and combined average for each year, it made my data frame very wide, so I
had to figure out how to consolidate it. At this point the columns I had 
were state, county, and then the rest or the columns I had just made using 
the split and drop methods. I wanted to make my data frame long to make it 
easier to manipulate in a dashboard, so I had to do what is called a melt. 
What this did was it took my very wide data frame and made it into only four 
columns. The first column being the state, the second being the county, the 
third being year combined with sex, and the last of being the value.
- What that did was take all of my data frames from 3191 rows 
and made them into 76,584 rows. From there I had to do another 
split of the combined column. Similar to before I had to make a separate
year and sex column put the correct values in each and delete the previously
combined column.
- From there I just had to check to make sure that the columns and rows 
lined up throughout all of the data frames and then I was finally able to 
pull them back into a CSV. Once I pulled them in I imported them to tableau 
where I could merge all of the CSV's together to start building my 
visualization.
-

## **Conclusion:**


## **Fun Facts:**
- The state of Delaware has the fewest amount of counties, it only has 3.
- The most common county name is Washington County, 31 states have this county.
- Louisiana is the only state to still have parishes and not counties. This is 
from the state being Roman Catholic under both Francis and Spain’s rule.
Through each change in history, they have never deviated from that.

## **Sources:**
[United States Life Expectancy and Age-specific Mortality Risk by County 1980-2014 | GHDx] (healthdata.org)




 
 ## **Key Notes:** 
- Probability of death in %, numbers are 95% uncertainty intervals.
- Life expectancy at birthin years, numbers are 95% uncertainty intervals.
