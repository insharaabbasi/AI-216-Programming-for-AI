**Program 1: Monthly Expense Check**

**What I did:**
I calculated the total monthly expenses for rent, food, transport, and utilities. Then I checked if the total goes above 60,000.

**Logic I used:**

* Add all expenses.
* Check if the total is more than 60,000 using if.
* Print a message depending on whether the total is safe or not.

**Problems I faced:**

* I forgot to call the function that checks the total, so the message didn’t show.
* I used sum as a variable, but Python has a built-in function sum.



**Program 2: Attendance Check**

**What I did:**
I checked which students are eligible based on their attendance. Students are eligible if attendance is more than 75%.

**Logic I used:**

* Go through each student’s attendance using a loop.
* Count students who are eligible and not eligible using two counters.

**Problems I faced:**

* I accidentally compared the whole list instead of one student at a time.
* The else statement was not correctly placed, so it gave wrong results at first.



**Program 3: Scholarship Eligibility**

**What I did:**
I found out how many students are eligible for a scholarship. Eligibility needs CGPA = 3.5 and family income = 80,000.

**Logic I used:**

* Use a loop to check each student’s CGPA and income.
* If both conditions are true, increase the eligible count.



**Problems I faced:**

* I printed the wrong variable name at the end (eligible\_count instead of eligible).
* I also had an unnecessary else that printed “Not Eligible” many times.



**Program 4: Sensor Alert System**

**What I did:**
I checked sensor readings to see which are outside the safe range (20–80). I counted alerts and calculated the percentage of unsafe readings.

**Logic I used:**

* Loop through readings and check if they are below 20 or above 80.
* Use a counter to count alerts.
* Calculate the percentage: (alerts / total readings) \* 100.

**Problems I faced:**

* At first, I used and instead of or in the condition, so no reading counted as alert.
* I tried sum(alerts) but alerts is a number, not a list.



**Program 5: General Counting / Analysis**

**What I did:**
I worked on different data like CGPA or attendance and counted totals or percentages to get useful information.

**Logic I used:**

* Loop through the data.
* Use counters to store totals.
* Use arithmetic to calculate percentages or averages.

**Problems I faced:**

* Remembering to use the correct logical operators (and / or).
* Keeping track of counters and variables correctly.
* Fixing small syntax mistakes and wrong variable names.





**Conclusion:**

1. These programs helped me learn:
2. How to use loops and if-else conditions.
3. How to count things with variables.
4. How to check conditions like safe ranges or eligibility.
5. How to debug mistakes like wrong variable names or logical errors.
6. This was a good practice for improving my Python logic and problem-solving skills.
