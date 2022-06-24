# Abstract

Python-written capability classifying - on different levels of Metrics : <br /> <br />
i- <ins> Active senior professional football players </ins> (*reference is season 2021/2022 at its end post Champions's League Final - not taking into account their retirement decision neither transfer for the next season*)  having won at least one Prestigious Major Title (*Chamipons's League, Nations World Cup, Nations Traditional European Championship, Nations Copa América (excluding Copa América Centenario), and Africa Cup of Nations*) <br /><br />
ii- <ins> Clubs for which they play </ins>, and <br /><br />
iii- <ins> Nations for which they play </ins>. <br /><br />


Moreover it provides a ***"Prominence Score"*** of the collected players based on a formula (Prominence is a function with *"Prizes Index"* and *"Age"* in the nomiator and *"Age"* squared in the denominator - as a probabilistic pattern or expression with additional factors in the formula and associated variables as well)  that uses both their *"Age"* and aforementioned Palmares a.k.a *"Prizes Index"*. 

Machine Learning techniques (*I know it can be simplified in saying - Statistical i/o ML - but I need to show off a bit like everyone else nowadays*) have been applied to the function to opimize it so that the final prominence is having a very low variance; i.e ˜ 1/1000 between the first and the second - that had not the same constellation of titles neither the same age - so un-biaised in nature)


# Scope and source of collected Data 

2021/2022 season (*2nd Half; i.e post-winter Transfer Window*) following squads : PSG, OL, LOSC, ASM, OM, MCY, LIV, CHE, MU, ARS, TOT, RM, FCB, ATM, BYM, BVB, BL, JUV, MIL, INT, NAP, and ATL (ATALANTA).         

Data Source = Wikipedia English.


P.S : None of the collected players have won an Asian Nations Cup, hence the absence of the Title from the analysis.


# Approach

- every single player from the above clubs is being checked whether he'd won any of the covered Honours, and how many of each if applies - the result is persisted in an observation (*i.o.w a record with the Player as a driver of the structured Data Points Model*), along with his MetaData; <br /><br />
- if the checked player hadn't won any - he's not persisted; <br /><br />
- the records are saved in a CSV file (*that I obviously won't share with you; neither the above-mentioned formulas btw*); <br /><br />
- a sample Custom-Weights-2-Models (*M1 and M2*) coefficients for each of the Titles is being assigned taking into account the complexity of the competition - Sorry Sadio and demonyms - (**Coefs.csv** *file available in the arborescence*). Note that the **M2** differs from **M1** only by annihilating the Champions's League Title - so assigning 0 to it. This **M2** corresponds then to only **continental prizes** ; <br /><br />    
- Off we go with running the code and obtaining the different results for both models.

# Insights

ABRACADABRA - To the Football Hard-Core Fans - Hereunder the most sensical discenring results (*To my taste*) : <br /><br />

**M1** <br /><br />

![M1_Players_Score_Age](https://user-images.githubusercontent.com/107439799/175091747-0f2c7483-a27e-49b9-8316-43493b6156ff.png)

![M1_Clubs_Score_Age](https://user-images.githubusercontent.com/107439799/175090652-92b2ab35-8765-4a18-938b-4611eca9d1c5.png)

![M1_Nations_Score_Age](https://user-images.githubusercontent.com/107439799/175090934-ccfc188e-7543-49cd-a1b1-d2091a58b4e1.png)

![M1_Players_Prom_Age](https://user-images.githubusercontent.com/107439799/175091901-e837d843-cc74-44da-959c-818c1402db52.png)


<img width="33%" alt="33 first prominent players" src="https://user-images.githubusercontent.com/107439799/175644844-e49dc595-c37f-42d0-8a78-889285202092.png">


**M2** <br /><br />

![M2_Players_Score_Age](https://user-images.githubusercontent.com/107439799/175093076-52dd85df-e9ac-423f-89b2-b312b8a00a84.png)

![M2_Clubs_Score_Age](https://user-images.githubusercontent.com/107439799/175093139-33b48f25-be98-4863-883c-9c4679fa544e.png)

![M2_Nations_Score_Age](https://user-images.githubusercontent.com/107439799/175093219-e0196a75-1b6d-469f-8179-130e76a53320.png)

![M2_Players_Prom_Age](https://user-images.githubusercontent.com/107439799/175093297-d3fa12a7-2a67-4383-97a6-02fa612e3ce4.png)



[Full results of both models M1 and M2](https://www.dropbox.com/sh/e0disjr3p93ypk3/AABh5YPoOQoxr0RAqF20eSrsa/Cloack-Room%20Prizes%20Index?dl=0&subfolder_nav_tracking=1)

