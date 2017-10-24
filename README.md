# Insight_DataChallenges
**Overview**<br>
Each week at Insight Health Data Science, we're offered a data challenge akin to what one might find during an interview process. Each involves one or more datasets and business problems which can be investigated through data science. We're instructed to spend no more than 4 hours on each (similar to what might be expected for a data challenge during the interview process).<br>
Each folder in this repository is dedicated to a single challenge. Within each folder can be found:<br>
1. The original challenge, usually in .pdf
2. The dataset(s), usually in .csv
3. My solution, a combination of code and descriptive Markdown contained in a Jupyter notebook<br>
**Challenge 1**<br> 
This challenge involved employee retention within several companies. Since turnover is expensive (given the amount of time and money it takes to find/hire/train a new employee to a skilled position), it's valuable to find out the reasons that employees leave and attempt to mitigate the ones that can be mitigated.<br>
My model for these data was a survival analysis (specifically, a Cox Proportional Hazards model), which identified the primary causes of employees leaving their companies to be salary, seniority, and department. Since seniority and department are difficult problems for companies to address, the key actionable item is salary increase, commensurate with the theoretical (or calculable from historical data) cost of hiring a new employee.<br><br> 
**Challenge 2**<br> 
This challenge involved a three-month-long A/B test between two different prices of an online sale. The business request was to determine which test made more money for the company and whether the test had gone on longer than necessary.<br>
I used a simple chi-squared test to determine whether the new price actually brought in more money than the standard price. As it turned out, no more complex model was necessary to answer the second question either; even with Bonferroni correction, using a chi-squared test each day showed the new price making more profit than the old within a week of starting the test.<br><br> 
**Challenge 3**<br> 
During this challenge, I investigated the conversion rate of customers and gave recommendations on how to increase that conversion rate. In addition to whether or not they converted, provided data about these users included their age, country (obtained from IP address), source (Ads, SEO, etc.), the total pages they visited on the site, and whether or not they were a new user.<br>
I used a decision tree to help visualize what the most impactful splits of the data would be, particularly focusing upon the age, country, and source, since these seemed actionable targets (as opposed to, e.g., how many pages a user viewed, which seemed difficult to influence in a meaningful way). I found that the company had a large number of visitors from China but a really terrible conversion rate with those users, and recommended that this sector be the focus of more targeted marketing.<br><br> 
