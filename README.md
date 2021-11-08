# Module 7: Pewlett Hackard Analysis
## Overview of the analysis
The purpose of this analysis is to help Bobby research Employee information at his company, Pewlett Hackard. He needs to find answers to the following questions:
- Who will be retiring in the next few years?
- How many positions will need to be filled?

To further help Bobby, we further analyze the employee data in our challenge exercise to determine the following:
- The number of retiring employees per title
- Identify employees who are eligible to participate in a mentorship program

## Results
![Retiring_Titles](https://github.com/Ellla12/Module-7-Pewlett-Hackard-Analysis/blob/main/Data/retiring_titles.PNG)

In Deliverable 1 we were tasked with determining the number of retiring employees per title. From the analysis, we can determine the following:
- There will be about 90,398 retirees who were born between 1952 and 1955.
- Senior Engineers and Senior Staff roles will be most impacted by this, as there will be 29414 and 28254 retirees respectively from each role.
- Managers are least impacted by retirement, as only 2 will be retiring.

![Mentorship Eligibilty](https://github.com/Ellla12/Module-7-Pewlett-Hackard-Analysis/blob/main/Data/mentorship_eligibilty.png)

In Deliverable 2 we were tasked with determining the number employees who are eligible to participate in a mentorship program. From the analysis, we can determine the following:
- There will be about 1,549 employees who will be eligible to participate in the mentorship program.

## Summary
1. How many roles will need to be filled as the "silver tsunami" begins to make an impact?
There will be 90,398 roles in need of being filled as soon as the "silver tsunami" starts retiring.

![Mentorship Count](https://github.com/Ellla12/Module-7-Pewlett-Hackard-Analysis/blob/main/Data/mentorship_count.png)

```
SELECT COUNT(title), title 
INTO mentorship_count
FROM mentorship_eligibilty
GROUP BY title
ORDER BY COUNT DESC;
```
2. Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?
Yes, there is plenty of retirement-ready employees in the departments to  mentor the next generation. We have 1,940 employees who are eligible to participate in a mentorship program and about 90,398 people who can mentor them before their retirement.
