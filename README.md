# Earnx Lottery on Moonbeam
Hi Moonbeam Community, see how you can win 50 GLMR prize !!! 

We decided to change our lottery schema. It not necessary to use Earnx Telegram Bot anymore and now all of ours delegators have a chance to win the lottery. 
For the next 4 weeks, we will run a lottery at Sunday 0h UTC given 50 GLMR for one of our delegators.

# Lottery Rules
- We will take an snapshot of all deletagors on the first network block after Sunday 0h UTC.
- You receive a number derivaded from your address representing a chance in the loterry.
- If you have delegated >= 200 GLMR, so you get another number increasing you chance.
- If you have made an aditional delegation >= 50 GLMR during the week (7 days before the sunday snapshot), you receive another number.

For example:
- You have delegated 200 GLMR in the past and delegated more 50 GLMR 5 days before lottery runs, so:
- You are one of ours delegators - 1 number
- You support us with more than 200 GLMR - 1 number
- You have delegated more 50 GLMR on last 7 days (before sunday lottery time): 1 number

# Lottery Winner
The Lottery is totaly transparent and deterministic, you can verify the results. The winner is defined by Math, so no one can cheat.

# Go now and delegate to EarnX to have a chance !!!

All Results will be published here and announced on Moonbeam Discord #General channel. 

# Next Lottery Runs 
Week 1 - on Sunday, January 23th, 2022 (open)

Week 2 - on Sunday, January 30th, 2022 (waiting)

Week 3 - on Sunday, February 06th, 2022 (waiting)

Week 4 - on Sunday, February 13th, 2022 (waiting)

( Maybe others Prize Week will come if this campaign is successful )

# Lottery Technical Details
Each participant on the lottery can have 1 , 2 or 3 numbers (chances) calculated as follow:<BR>
We starting assuming we will use numbers with X bytes (X = 4 on first try, so 32 bits numbers)
- Number1 is the last X bytes of deletegator address (using hexadecimal string)
- Number2 is the last X bytes of sha256(number1 using hexadecimal string)
- Number3 is the last X bytes of sha256(number2 using hexadecimal string)
- Lucky number is the last X bytes of first network block hash (using hexadecimal string) after Sunday 0h UTC. 
The winner is who have the closer number of Lucky Number.
If there is any number collision when generating participants numbers, we increase X by 1 and repeat all the calculations again.





 
