# Pewlett-Hackard-Analysis

## Overview
In prepartion of the "Silver Tsunami", in other words, the aging workforce, I was tasked to create tables to determine employees that were reaching retirement age and to identify employees who are eligible to particiapte in the Pewlett Hackard mentorship program. I was able to complete these two task by using PostgreSQL.

## Results

- How many employees are eligible to retire?
  - As part of the first task, I created a table called retiring_tables which retrieves the count of employees that are eligible to retire grouped by job titles. In order to be eligble to retire, the employee must be born between 1952 and 1955. It must be mentioned that there are 300,024 employees at Pewlett Hackard. In total, 90,398 employees are eligible to retire out of 300,024 employees meaning about 30% of Pewlett Hackard workforce are elgible to retire.
  - <img width="228" alt="retirement_eligible" src="https://user-images.githubusercontent.com/91519293/145734260-8c0d0b71-4269-4fc3-acde-30df01e7d42d.png">
- Retirement by Job Title
  - The majority of the employees eligible to retire hold senior positions with senior engineers having the most amount of employees at retirement age. To be exact, 57,668 employees out of 90,398 hold senior job titles which equates to nearly 64% employees at retirement age are in senior positions. Interestingly, 2 managers are at retirement age.
- Breakdown by Job Title
  - By number of employees reaching retirement age and by job title: 29414 Senior Engineers, 28254 Senior Staff, 14222 Engineers, 12243 staff, 4502 Technique Leaders, 1761 Assistant Engineers, and 2 Managers. The roles of Senior Engineers and Senior Staff should be prioritized to filled.
- Mentorship Eligibility
  - For the second task, I created a table called mentorship_eligibilty which retrieves each employee's employee number, first name, last name, birth date, their hire date, the last day of employment, and their job title that were born in 1965. The query used returned 1549 employees that were eligible to participate in the mentorship program. With a total of 300,024 employees, only 1549 employees are eligible become mentors making up 0.5% of the total workforce at Pewlett Hackard. 
  - <img width="734" alt="mentorship_eligible" src="https://user-images.githubusercontent.com/91519293/145735795-47edf8ea-eb97-4c91-b926-fbb098ddfdc2.png">
## Analysis

- How many roles will need to be filled as the "silver tsunami" begins to make an impact?
  - Recalling to the results section, there were 90,398 employees eligible to retire. Over half the number of employees ready to retire are in senior positions. There is not concrete number that can determined, but a priotization filling senior engineers and senior staff roles should be made to reduce the impact of "silver tsunami".
- Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?
  - I think that there is not enough mentorship eligible employees to mentor the next generation of Pewlett Hackard employees, for there are only 1549 employees eligible with 300,024 total employees. To allow for more mentors to accomodate the large workforce, I think that broadening the critieria that qualifies employees to be eligible from being born in 1965 to range of years. For example, a modification on the filter on the original query to allow employees born from 1962-1965 would allow for 56,859 employees eligible to mentor the next generation.
  - <img width="228" alt="retirement_eligible" src="https://user-images.githubusercontent.com/91519293/145738556-7dee3d0c-a78e-4910-8150-8936e9deda53.png">
