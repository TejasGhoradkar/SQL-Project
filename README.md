# SQL-PROJECT

Bidding on batters
(1) get 2-3 players with high S.R who have faced at least 500 balls.And
to do that you have to make a list of 10 players you want to bid in the auction so that
when you try to grab them in auction you should not pay the amount greater than you
have in the purse for a particular player.
(strike rate is total runs scored by batsman divided by number of balls faced but remember
when extras_type is 'wides' it is not counted as a ball faced neither counted as batsmen runs)

(2) get 2-3 players with good Average who have played more than 2 ipl
seasons. And to do that you have to make a list of 10 players you want to bid in the
auction so that when you try to grab them in auction you should not pay the amount
greater than you have in the purse for a particular player.
(Average is calculated as total runs scored divided by number of times batsman has been
dismissed which can be calculated using wicket_ball field as 1 indicates out and 0 indicates not
out, a batsman should’ve been dismissed at least once to calculate the sr i.e., you can exclude
those players who have not been dismissed once )

(3) get 2-3 Hard-hitting players who have scored most runs in boundaries
and have played more the 2 ipl season. To do that you have to make a list of 10 players
you want to bid in the auction so that when you try to grab them in auction you should
not pay the amount greater than you have in the purse for a particular player.
(only 4 and 6 will be counted as boundaries so calculate how many 4 and 6 has been hit by
each batsman and also calculate total runs scored to get the output as boundary percentage
which will be runs in boundary divided by total runs scored)

Bidding on Bowlers
(1) get 2-3 bowlers with good economy who have bowled at least 500
balls in IPL so far.To do that you have to make a list of 10 players you want to bid in the
auction so that when you try to grab them in auction you should not pay the amount
greater than you have in the purse for a particular player.(economy can be calculated by
dividing total runs conceded with total overs bowled)

(2) get 2-3 bowlers with the best strike rate and who have bowled at least
500 balls in IPL so far.To do that you have to make a list of 10 players you want to bid in
the auction so that when you try to grab them in auction you should not pay the amount
greater than you have in the purse for a particular player.
(strike rate of a bowler can be calculated by number of balls bowled divided by total wickets
taken )

All-Rounders

(1) get 2-3 All_rounders with the best batting as well as bowling strike rate
and who have faced at least 500 balls in IPL so far and have bowled minimum 300
balls.To do that you have to make a list of 10 players you want to bid in the auction so
that when you try to grab them in auction you should not pay the amount greater than
you have in the purse for a particular player.
( strike rate of an all rounder can be calculated using the same criteria of batsman similarly the
bowling strike rate can be calculated using the criteria of a bowler)

Wicketkeeper
Now, after adding all these players, this team is still incomplete because we don’t have any
wicketkeeper. In T20 cricket, the role of the wicketkeeper is slightly different from that in longer
forms of the game. In T20, the emphasis is on scoring runs quickly, so the wicketkeeper is often
expected to contribute to the team's run total with aggressive batting. They may also be called
upon to bowl a few overs of spin or medium pace.
Defensively, the wicketkeeper still has an important role to play, as they are responsible for
catching and stumping the batsman. In T20 cricket, where every run and wicket is crucial, a
good wicket keeper can make a big difference to the team's chances of winning.
Overall, the wicketkeeper is an important member of a T20 team and can have a significant
impact on the outcome of a match. Now suppose you are provided with a list of wicketkeeper
names, and your task is to define the criteria for choosing the two best wicket keepers from all
those names.Try to define a criteria best suited for a wicketkeeper required in a t20 team so that
your team will be complete and have everything required for winning this year’s IPL

Additional Questions 
NOTE:-Deliveries is the table created using the IPL_Ball data whereas the Matches table has been
created using the IPL_Matches data
1. Get the count of cities that have hosted an IPL match
2. Create table deliveries_v02 with all the columns of the table ‘deliveries’ and an additional
column ball_result containing values boundary, dot or other depending on the total_run
(boundary for >= 4, dot for 0 and other for any other number)
(Hint 1 : CASE WHEN statement is used to get condition based results)
(Hint 2: To convert the output data of the select statement into a table, you can use a
subquery. Create table table_name as [entire select statement].
3. Write a query to fetch the total number of boundaries and dot balls from the
deliveries_v02 table.
4. Write a query to fetch the total number of boundaries scored by each team from the
deliveries_v02 table and order it in descending order of the number of boundaries
scored.
5. Write a query to fetch the total number of dot balls bowled by each team and order it in
descending order of the total number of dot balls bowled.
6. Write a query to fetch the total number of dismissals by dismissal kinds where dismissal
kind is not NA
7. Write a query to get the top 5 bowlers who conceded maximum extra runs from the
deliveries table
8. Write a query to create a table named deliveries_v03 with all the columns of
deliveries_v02 table and two additional column (named venue and match_date) of venue
and date from table matches
9. Write a query to fetch the total runs scored for each venue and order it in the descending
order of total runs scored.
10. Write a query to fetch the year-wise total runs scored at Eden Gardens and order it in the
descending order of total runs scored.
