# 1st Place Solution

This is a repository in which I share my approach/solution and correspoding scripts for 1st place solution of machine learning competition "[March Machine Learning Mania 2022 - Women's](https://www.kaggle.com/competitions/womens-march-mania-2022)".

First of all, I'd like to thank kaggle admins for hosting this year's competittion. This is my second time participation into NCAA Basketball competitions hosted on kaggle. As well as last year's competition, it was quite enjoyable to watch games and check how my models work every day. I'd like to thank kaggle admins for orgnazing this competition.

In this repository/forum, I'd like to share my approach to this year's competition. However this type of competition is heavily influenced by luck, so my aproach would not work next year by high chance. But, I hope some of you find my approach useful.

Basically, I subimmited two types of models. One of them is "passive" model, the other is "aggressive/gambling" model.
In short, my agressive/gambling model ended up being the most accurate model throughout the competition. Although my passive model didn't work as well as the other one, still brought me better result than I expected. (In fact the final leaderboard score was 0.43574, bronze medal.) 

In "passive" model, I submitted predition calculated using LightGBM without any post-processing. 
In "agressive/gambling" model, I did override predicition of three teams.

[Data Preparation]
I wrote R scripts code to set up datasets. 
I did no tricky things at all, I setup very basic features such as Seed info, teamid, team information...
For further complete information, please read my [R codes](https://github.com/koki25ando/March-Machine-Learning-Mania-2022---Women-s/tree/master/R_code) which exist in 'R' folder in this repo.

[Modeling]
I used only one model, LightGBM. That's it. I didn't even stacked any other models in the end.
I tried to make it as simple as possible. So I decided use only LightGBM.
See [this notebook](https://github.com/koki25ando/March-Machine-Learning-Mania-2022---Women-s/blob/master/py/LightGBM_stage2.ipynb) for more information.

[Post-Processing]
Here comes aggressive/gambling part. Basically i did override 3 teams prediction as every other participants in this competitions do.
I've read some articles, and chose three teams, "Stanford", "Uconn", "South Carolina".
In the end, three of them survived until FINAL FOUR. I guess I was just this year's lucky boy.