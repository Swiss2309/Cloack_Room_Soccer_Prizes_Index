# Abstract

Python-written capability classifying - on different levels of Metrics : <br /> <br />
i- Active senior professional football players (reference is season 2021/2022 at its end post Champions's League Final - not taking into account their retirement decision neither transfer for the next season)  having won at least one Prestigious Major Title (Chamipons's League, Nations World Cup, Nations Traditional European Championship, Nations Copa América (excluding Copa América Centenario), and Africa Cup of Nations) <br /><br />
ii- Clubs for which they play, and <br /><br />
iii- Nations for which they play. <br /><br />

Moreover it provides a ***"Prominence Score"*** of the collected players based on a formula (Prominence is a function with *"Prizes Index"* and *"Age"* in the nomiator and *"Age"* squared in the denominator - as a probabilistic pattern or expression with additional factors in the formula and associated variables as well)  that uses both their *"Age"* and aforementioned Palmares a.k.a *"Prizes Index"*. 

Machine Learning techniques (I know it can be simplified in saying - Statistical i/o ML - but I need to show off a bit like everyone else nowadays) have been applied to the function to opimize it so that the final prominence is having a very low variance; i.e ˜ 1/1000)
 
# Scope and source of collected Data 

2021/2022 season (2nd Half; i.e post-winter Transfer Window) following squads : PSG, OL, LOSC, ASM, OM, MCY, LIV, CHE, MU, ARS, TOT, RM, FCB, ATM, BYM, BVB, BL, JUV, MIL, INT, NAP, and ATL.         

Data Source = Wikipedia English.


P.S : None of the collected players have won an Asian Nations Cup, hence the absence of the Title from the analysis.


# Approach

- every single player from the above clubs is being checked whether he'd won any of the covered titles, and how many of each if applies - the result is persisted in an observation (*i.o.w a record with the Player as a driver of the structured Data Points Model*), along with his MetaData; <br /><br />
- if the checked player hadn't won any - he's not persisted; <br /><br />
- the records are saved in a CSV file (*that I obviously won't share with you*); <br /><br />
- a sample Custom-Weights-2-Models (M1 and M2) Coefficients for each of the Titles is being assigned taking into account the complexity of the competition (**Coefs.csv** *file available in the arborescence*). Note that the **M2** differs from **M1** only by annihilating the Champions's League Title - so assigning 0 to it. This **M2** corresponds then to only **continental prizes** ; <br /><br />    
- Off we go with running the Program and obtaining the different results for both models.

# Insights

Hereunder the most discenring results (*To my taste*) : <br /><br />


[Full results of both models M1 and M2](https://www.dropbox.com/sh/e0disjr3p93ypk3/AABh5YPoOQoxr0RAqF20eSrsa/Cloack-Room%20Prizes%20Index?dl=0&subfolder_nav_tracking=1)

