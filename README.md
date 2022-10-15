# Abstract

Python-written capability classifying - on different levels of Metrics : <br /> <br />
i- <ins> Active senior professional (Men) football players </ins> (*reference is season 2021/2022 at its end post Champions's League Final - not taking into account their retirement decision neither transfer for the next season*)  having won at least one Prestigious Major Title (*Champions's League, Nations World Cup, Nations Traditional European Championship, Nations Copa América (excluding Copa América Centenario), and Africa Cup of Nations*) <br /><br />
ii- <ins> Clubs for which they play </ins>, and <br /><br />
iii- <ins> Nations for which they play </ins>. <br /><br />


Moreover it provides a ***"Prominence Score"*** of the collected players based on a formula with *"Prizes Index"* and *"Age"* in the nomiator and *"Age"* squared in the denominator - as a probabilistic pattern expression with additional weighting factors. <br /><br />

<img width="560" alt="Screenshot 2022-07-05 at 2 20 34 pm" src="https://user-images.githubusercontent.com/107439799/177326333-d7a06fe1-a20d-4455-8ee3-2d0654899c9a.png">

Statistical hyper-parameter tuning have been applied to the formula to optimize it so that the final prominence is having a very low variance; i.e ˜ 1/1000 between the first and the second - that had not the same constellation of titles neither the same age - so un-biaised in nature - c.f the Table just underneath the Prominence plot.


# Scope and source of collected Data 

**2021/2022 season** (*2nd Half; i.e post-winter Transfer Window*) following squads : **PSG, OL, LOSC, ASM, OM, MCY, LIV, CHE, MU, ARS, TOT, RM, FCB, ATM, BYM, BVB, BL, JUV, MIL, INT, NAP, and ATL** (*ATALANTA, not Atlético, already mentioned under ATM code*).         

<ins>Data Source</ins> = **Wikipedia English**.


P.S : None of the collected players have won an Asian Nations Cup, hence the absence of the Title from the analysis.


# Approach

- every single player from the above clubs is being checked whether he'd won any of the covered Honours, and how many of each if applies - the result is persisted in an observation (*Player as a driver of the structured Data Points Model*), along with his MetaData; <br /><br />
- if the checked player hadn't won any - he's not persisted; <br /><br />
- the records are saved in a CSV file - in Total 161 players made it to the CSV; respresenting 30 Nations (**Palmares.csv** *file available in the arborescence*); <br /><br />
- a sample Custom-Weights-2-Models (*M1 and M2*) coefficients for each of the Titles is being assigned taking into account the ferocity of the competition - Sorry Sadio and demonyms - (**Coefs.csv** *file available in the arborescence and below its content*). 

<img width="496" alt="Screenshot 2022-07-05 at 3 02 36 pm" src="https://user-images.githubusercontent.com/107439799/177334283-7828a233-fb0f-47db-864a-e221f1fcd8ca.png">

Note that the **M2** differs from **M1** only by annihilating the Champions's League Title - so assigning **0** to it. This **M2** corresponds then to only **Nations continental palmares** ; <br />

- Off we go with running the code and obtaining the different results for both models.

# Insights

ABRACADABRA - To the Football Hard-Core Fans - Hereunder the most sensical germane results (*To my taste*) : <br />

**M1** <br />

![M1_Players_Score_Age](https://user-images.githubusercontent.com/107439799/175091747-0f2c7483-a27e-49b9-8316-43493b6156ff.png)

Note that only **G. PIQUE** hadn't played for **Real Madrid** from above list. <br /><br />

Also - **MESSI** is 15th in the List, preceeded by **MODRIC** (*12th*), **VARANE** (*13th*), and **BUSQUETS** (*14th*) - surprisingly - or not; whereas **CR7** is 3rd. This is called **Legacy**. (*Addendum : MESSI'd lost 10 finals across all competitions; of which 4 from our covered Index*). <br /><br />

![M1_Clubs_Score_Distribution](https://user-images.githubusercontent.com/107439799/175783072-0048771d-0289-44d2-bb85-04b018a39287.png)

![M1_Nations_Score_Distribution](https://user-images.githubusercontent.com/107439799/175783242-7ba49d24-3bb4-499a-81fd-928dc0bd6211.png)

![M1_Players_Prom_Age](https://user-images.githubusercontent.com/107439799/175091901-e837d843-cc74-44da-959c-818c1402db52.png)

Below is the 33 most prospect players (*33 = 3 * 11 - i.e 3 Teams*) <br />

<img width="33%" alt="33 first prominent players" src="https://user-images.githubusercontent.com/107439799/175769437-7efc3fee-5c2f-47ec-9a06-999eb569bf63.png"> <br />

Aggregated on **Club** Level - The 10 most prominent Clubs are as follows :  <br />

![M1_Clubs_Prominence](https://user-images.githubusercontent.com/107439799/176651051-acbce05d-bd14-4522-aea3-9bd4226b1b14.png) <br />

And on **Nation's** : <br />

![M1_Nations_Prominence](https://user-images.githubusercontent.com/107439799/176651240-e671d0d2-94e4-40f8-8b63-906dedf81ced.png) <br /><br />


**M2** <br />

![M2_Players_Score_Age](https://user-images.githubusercontent.com/107439799/175093076-52dd85df-e9ac-423f-89b2-b312b8a00a84.png)

![M2_Clubs_Score_Distribution](https://user-images.githubusercontent.com/107439799/175784010-88d17ce0-4e28-4d46-84c1-b8aed66dd613.png)

Pause in a second - where's **Real Madrid** here ? Interesting - isn't it ? They are in the 15th rank in effect on this pure Nations Continental Level - This is Data speaking. <br /><br />


![M2_Nations_Score_Distribution](https://user-images.githubusercontent.com/107439799/175784019-37504748-da66-4955-a184-1757551fdb87.png)


Hello **Sadio et al !!** <br /><br />

![M2_Players_Prom_Age](https://user-images.githubusercontent.com/107439799/175093297-d3fa12a7-2a67-4383-97a6-02fa612e3ce4.png)

Below is the 33 most prospect players (*33 = 3 * 11 - i.e 3 Teams*) <br />

<img width="30%" alt="33 first prominent players" src="https://user-images.githubusercontent.com/107439799/175647347-416a35dc-112c-4236-92cf-2414907d3057.png">   <br />


Aggregated on **Club** Level - The 10 most prominent Clubs are as follows :  <br />

![M2_Clubs_Prominence](https://user-images.githubusercontent.com/107439799/176651967-66ce779d-007c-43e7-ad29-4ea0774e87b1.png) <br />

And on **Nation's** : <br />

![M2_Nations_Prominence](https://user-images.githubusercontent.com/107439799/176652116-024eaf77-9277-4555-a3d6-7584ec163bbf.png)

 <br />


[**Full results of both models M1 and M2**](https://bit.ly/3P6xYAb) <br /><br />

***To be continued (Or not)...***
