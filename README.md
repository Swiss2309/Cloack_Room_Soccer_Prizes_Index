# Abstract

Python-written capability classifying : 
i- active senior professional football players (reference is season 2021/2022 at its end post Champions's League Final - not taking into account their retirement decision neither transfer for the next season)  having won at least one Prestigious Major Title (Chamipons's League, Nations World Cup, Nations Traditional European Championship, Nations Copa América (excluding Copa América Centenario), and Africa Cup of Nations)
ii- Clubs for which they play, and
iii- Nations for which they play.

Moreover it provides a "Prominence Score" of the collected players based on a formula (Prominence is a function with "Prizes Index" and "Age" in the nomiator and "Age" squared in the denominator - as a pattern)  that uses both their "Age" and aforementioned Palmares a.k.a "Prizes Index". 

Machine Learning techniques (I know it can be simplified in saying - Statistical i/o ML - but I need to show off a bit like everyone else nowadays) have been applied to the function to opimize it so that the final prominence is having a very low variance; i.e ˜ 1/1000)
 
# Scope and source of collected Data 

2021/2022 season (2nd Half; i.e post-winter Transfer Window) following squads : PSG, OL, LOSC, ASM, OM, MCY, LIV, CHE, MU, ARS, TOT, RM, FCB, ATM, BYM, BVB, BL, JUV, MIL, INT, NAP, and ATL.         

Data Source = Wikipedia English.


P.S : None of the collected players have won an Asian Nations Cup, hence the absence of the Title from the analysis.


# Approach
Custom Weights used in probabilistic expressions.

# Insights

[Full results of both models M1 and M2](https://www.dropbox.com/sh/e0disjr3p93ypk3/AABh5YPoOQoxr0RAqF20eSrsa/Cloack-Room%20Prizes%20Index?dl=0&subfolder_nav_tracking=1)

