# Abstract

Python-written capability classifying - on different levels of Metrics : <br /> <br />
i- <ins> Active senior professional football players </ins> (*reference is season 2021/2022 at its end post Champions's League Final - not taking into account their retirement decision neither transfer for the next season*)  having won at least one Prestigious Major Title (*Chamipons's League, Nations World Cup, Nations Traditional European Championship, Nations Copa América (excluding Copa América Centenario), and Africa Cup of Nations*) <br /><br />
ii- <ins> Clubs for which they play </ins>, and <br /><br />
iii- <ins> Nations for which they play </ins>. <br /><br />


Moreover it provides a ***"Prominence Score"*** of the collected players based on a formula (Prominence is a function with *"Prizes Index"* and *"Age"* in the nomiator and *"Age"* squared in the denominator - as a probabilistic pattern or expression with additional factors in the formula and associated variables as well)  that uses both their *"Age"* and aforementioned Palmares a.k.a *"Prizes Index"*. 

Machine Learning techniques (*I know it can be simplified in saying - Statistical i/o ML - but I need to show off a bit like everyone else nowadays*) have been applied to the function to opimize it so that the final prominence is having a very low variance; i.e ˜ 1/1000 between the first and the second - that had not the same constellation of titles neither the same age - so un-biaised in nature - c.f the Table just underneath the Prominence plot)


# Scope and source of collected Data 

2021/2022 season (*2nd Half; i.e post-winter Transfer Window*) following squads : PSG, OL, LOSC, ASM, OM, MCY, LIV, CHE, MU, ARS, TOT, RM, FCB, ATM, BYM, BVB, BL, JUV, MIL, INT, NAP, and ATL (ATALANTA).         

Data Source = Wikipedia English.


P.S : None of the collected players have won an Asian Nations Cup, hence the absence of the Title from the analysis.


# Approach

- every single player from the above clubs is being checked whether he'd won any of the covered Honours, and how many of each if applies - the result is persisted in an observation (*i.o.w a record with the Player as a driver of the structured Data Points Model*), along with his MetaData; <br /><br />
- if the checked player hadn't won any - he's not persisted; <br /><br />
- the records are saved in a CSV file (*that I obviously won't share with you; neither the above-mentioned formulas btw*) - in Total 162 players made it to the CSV; <br /><br />
- a sample Custom-Weights-2-Models (*M1 and M2*) coefficients for each of the Titles is being assigned taking into account the complexity of the competition - Sorry Sadio and demonyms - (**Coefs.csv** *file available in the arborescence*). Note that the **M2** differs from **M1** only by annihilating the Champions's League Title - so assigning 0 to it. This **M2** corresponds then to only **continental prizes** ; <br /><br />    
- Off we go with running the code and obtaining the different results for both models.

# Insights

ABRACADABRA - To the Football Hard-Core Fans - Hereunder the most sensical discenring results (*To my taste*) : <br /><br />

**M1** <br /><br />

![M1_Players_Score_Age](https://user-images.githubusercontent.com/107439799/175091747-0f2c7483-a27e-49b9-8316-43493b6156ff.png)

Note that only **G. PIQUE** hadn't played for Real Madrid from above list. <br /><br />

![M1_Clubs_Score_Distribution](https://user-images.githubusercontent.com/107439799/175783072-0048771d-0289-44d2-bb85-04b018a39287.png)

![M1_Nations_Score_Distribution](https://user-images.githubusercontent.com/107439799/175783242-7ba49d24-3bb4-499a-81fd-928dc0bd6211.png)

![M1_Players_Prom_Age](https://user-images.githubusercontent.com/107439799/175091901-e837d843-cc74-44da-959c-818c1402db52.png)

Below is the 33 most prospect players (*33 = 3 * 11 - i.e 3 Teams*) <br /><br />

<img width="33%" alt="33 first prominent players" src="https://user-images.githubusercontent.com/107439799/175769437-7efc3fee-5c2f-47ec-9a06-999eb569bf63.png">



**M2** <br /><br />

![M2_Players_Score_Age](https://user-images.githubusercontent.com/107439799/175093076-52dd85df-e9ac-423f-89b2-b312b8a00a84.png)

![M2_Clubs_Score_Distribution](https://user-images.githubusercontent.com/107439799/175784010-88d17ce0-4e28-4d46-84c1-b8aed66dd613.png)

As **PSG Big Fan** the above is my sought-after graph when the idea of this feature got incepted into my mind. Happy to have confirmed what I was projecting - right after **SENEGAL** won the Africa cup of Nations (represented by **Idrissa Gana** and **Abdou Diallo**). <br /><br />


![M2_Nations_Score_Distribution](https://user-images.githubusercontent.com/107439799/175784019-37504748-da66-4955-a184-1757551fdb87.png)

![M2_Players_Prom_Age](https://user-images.githubusercontent.com/107439799/175093297-d3fa12a7-2a67-4383-97a6-02fa612e3ce4.png)

Below is the 33 most prospect players (*33 = 3 * 11 - i.e 3 Teams*) <br /><br />

<img width="30%" alt="33 first prominent players" src="https://user-images.githubusercontent.com/107439799/175647347-416a35dc-112c-4236-92cf-2414907d3057.png">


[Full results of both models M1 and M2](https://www.dropbox.com/sh/e0disjr3p93ypk3/AABh5YPoOQoxr0RAqF20eSrsa/Cloack-Room%20Prizes%20Index?dl=0&subfolder_nav_tracking=1)

