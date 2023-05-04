Download Link: https://assignmentchef.com/product/solved-csci-4380-homework-4
<br>
Database Systems

For this assignment, you will construct a single SQL query to generate the answer to each of the below ques­tions. Use the baseball database (<a href="https://gitlab.com/samuelbjohnson/baseball)">https://gitlab.com/samuelbjohnson/baseball</a><u>)</u> introduced in class.

You should put your answers in a series of .sql files, each named with the number of the question it answers (1.sql, 2.sql, etc.), and then upload all of your solutions to Submitty. The assignment will be auto-graded, expecting an exact match for output. The auto-grader will consider only the first valid SQL statement in each file. A schema, specifying name and order of columns, is provided for each question.

Default Submitty rules for multiple submissions will apply (you get twenty free attempts, after that, each additional attempt will cost you 0.1 points up to a maximum of 5 points).

A few useful notes and clarifications:

<ul>

 <li>Batting average is defined as h/ab (hits divided by at-bats)</li>

 <li>Salary data is only available starting in 1985. Any questions that involve salary information assume a natural join (i.e., don’t try to pull in data from years without salary data).</li>

 <li>Players are chosen for the ”All Star Game” each year. A given player may appear in the all star game in multiple years.</li>

</ul>

Query efficiency isn’t considered, except that the total runtime for all of your queries is capped, and the queries are run in numerical order. Therefore, a query that is too slow may cause the process to timeout, leading to no credit for that and subsequent queries.




<ol>

 <li>The number of pitchers with more than (&gt;) 40 saves (sv) in a single year since (&gt;=) 1975. Note that a pitcher may play multiple stints in a given year. (count)</li>

 <li>The number of players under 6 feet (&lt; 72inches) whose batting average was above .300 in 1995. Note that integer arithmetic will apply and needs to be taken into account. Ignore players with fewer than 50 at-bats. (count)</li>

 <li>List the years since (&gt;=) 1975 where the manager with the most wins also managed the team that won their division (divwin), in descending order with the earliest year last. (years)</li>

 <li>The combined team salaries for each year’s world series winner in descending order, with the highest combined team salary first. (year, salary)</li>

 <li>Franchise name and average total yearly franchise attendance from (&gt;=) 1997 to the present (use atten­dance from teams table, and don’t worry about the attendance of games played elsewhere) (franchise, attendance)</li>

 <li>First and last name and number of All Star appearances by the eight players on the ballot for the Hall of Fame in 2000 with the most All Star appearances, using the number of votes received as a tie-breaker if needed. Note that having a tuple in the halloffame table for a given year indicates that a player is on the ballot for that year, and that having a tuple in the allstarfull table indicates an All Star appearance (this does not require use of the appearances table). (first, last, appearances)</li>

</ol>




<ol start="7">

 <li>Career (total) batting average (label the column career avg) of players born between 1958 and 1960, inclusive, who have more than 300 at-bats, ordered by average, highest to lowest. (playerid, career avg)</li>

 <li>Ratio of average All Star player salaries to average player salaries for each year, in order of year, earliest years first. (year, ratio)</li>

 <li>Average combined team salary for each year, in order of year, earliest years first. (year, salary)</li>

 <li>The school name and number of All Star players for the ten colleges with the most All Star players. List the school with the most players first. A player counts as an All Star player regardless of how many times they’ve played in the All Star game. In case of ties, use the school name in alphabetical order. (school name, count)</li>

 <li>The park names (park) that do not include “field”, “park”, or “stadium” for teams that won their division series (use the seriespost table for this). (park)</li>

 <li>The names of the teams that have lost more than 2 (&gt;) league championships. (name)</li>

 <li>The first and last name of players who have a second stint where they had more at-bats (&gt;) but fewer hits (&lt;) than their first stint of the same year, in order from heaviest to lightest weight. (first, last)</li>

 <li>The awards (use awardid) that were won by the same player three consecutive years between 1950 and 1959, inclusive. (award)</li>

 <li>The first and last name and birth city of all players who were born in New York State and played for the New York Yankees franchise (franchid=’NYY’). (first, last, city)</li>

</ol>