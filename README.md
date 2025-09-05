# Football Analytics

This repo contains the projects, tools, and resources for football data analysis & visualisation. Commonly used tools include Python, Web Scraping, NumPy, Pandas, Matplotlib, Seaborn, and Jupyter Notebook. Several visuals from various projects can also be found on Twitter ([@thatderekchui](https://x.com/thatderekchui)).

Click on the arrows to select and expand each project for more details!

## Contents

### Regularly Updated
- [Match Reviews](#match-reviews)
- [Player Dashboard](#player-dashboard)

### Featured Projects
- [(In Progress) Project 3 - Outlying Player Valuations](#3---outlying-player-valuations)
- [Project 2 - 2025 Summer Squad Assessment](#2---2025-summer-squad-assessment)
- [Project 1 - Progression Analysis (24/25)](#1---progression-analysis-2425)

### Personal Favorites
<details>
  <summary>2.3 - Replacing Cunha</summary>

  - **Code**: [project2-3.ipynb](./Project%202/Project%202.3/project2-3.ipynb)  
  - **Summary**:  
    With Cunha leaving to United, I'm interested to see how Wolves will replace the 62.5m euro man. And realistically, his stats won't be replicated at Wolves for a while. Out of all 10 categories, when compared to departing, current, and rumored Wolves players (12), Cunha tops 4 of them, and is 3rd in two others. With a +6.4 difference in non penalty goals and expected goals, the next closest of the bunch is Akturkoglu with +1.3, who stands out as one of the best replacements, and would play well along side the likes of Arias and Lopez. As seen below, he also has the most podium finishes after Cunha.

  <p align="center">
    <img src="./Project%202/Project%202.3/2-3-1.png" alt="2.3" width="75%" />
  </p>

  We can highlight these players (another good pick would be Ben Doak) and split them by shooting, progression, and pressing. It's easy to notice the similarities between Matheus and Kerem. Identical expected goal contributions and shots on target per 90, similar progressively and both fairly aggressive. Despite his lower take ons and npG-xG, Kerem makes up for in touches in the opposite pen and interceptions. Again Ben Doak shares similar stats in the Championship last season. I believe these two are arguably better picks than the likes of Amine Adli and Matthis Abline, both who are more popular choices. 

  <p align="center">
    <img src="./Project%202/Project%202.3/2-3-2.png" alt="2.3" width="75%" />
  </p>

  Here Cunha and Akturkoglu both are the only shot dominant players, which is something we're lacking after Cunha imo. Bellegarde and Munetsi provide depth to both midfield and CAM, hence their press heavy characteristics, espeically for attacking players. Progressive architypes are pretty common, since Wolves already have Arias and Lopez, but Doak would be a good addition as well. Adli and Abline are good too but I would personally perfer Kerem and Ben. That way, Wolves would have a Cunha like player and sufficient progressive options (as well as press heavy like Munetsi).

  <p align="center">
    <img src="./Project%202/Project%202.3/2-3-3.png" alt="2.3" width="75%" />
  </p>

  Below are further metrics and distributions of all the players referenced and used for comparison.

  <p align="center">
    <img src="./Project%202/Project%202.3/2-3-4.png" alt="2.3" width="75%" />
  </p>

</details>

<details>
  <summary>Matchweek 1 Review: City (Home)</summary>

  - **Code**: [postMatchweek1.ipynb](./match-reviews/Matchweek%201/postMatchweek1.ipynb)  
  - **Summary**:
    Despite the dissappointing 0-4 result, I believe it's revealing and there's a lot of new insights we can take from this game. Apart from a few major mistakes at the back, the team didn't look to bad imho.

    I'm suprised how central our attack was compared to last time we played city. A 48% centrality bias compared to last time's 13%. A few shots from Munetsi's offside as well as Larsen. Note that all these shows are clustered very close together as well. What impressed me however was Hoever, who not only dealt with Doku fairly well with Doherty (especially compared to last time) and made several progressive passes and crosses on the bottom wing of the graph. In fact, all 4 SCA crosses originated from the right side.
    
    Part of me wonders if there would've been better chances for Larsen if those crosses from the right were passes instead.

    What's concerning is the lack of progression from the left hand side / top wing. Wolfe and Bellegarde didn't contribute much to the attack. Neither did Hugo Bueno later on.

  <p align="center">
    <img src="./match-reviews/Matchweek%201/4-1-5.png" alt="4.1" width="75%" />
  </p>

  City also attacked fairly centrally, especially compared to last time. Obviously this is because of Haaland returning vs City playing KDB up top before. Fairly even distribution in passing. Less action on the left / top wing from Doku as mentioned. Much deeper build up play compared to us, but tbf that's what you expect from a team like City.

  <p align="center">
    <img src="./match-reviews/Matchweek%201/4-1-6.png" alt="4.1" width="75%" />
  </p>

  I mean the results speak for themselves on the plot below. Our options on the bench aren't bad either: Mosquera, Hugo Bueno, Rodrigo Gomes, Arias, Lopez, as well as Tchatchoua coming in soon. Hopefully it will only be up from here and both Agbadou & Sa gets in the right mindset.

  <p align="center">
    <img src="./match-reviews/Matchweek%201/4-1-7.png" alt="4.1" width="75%" />
  </p>

  <p align="center">
    <img src="./match-reviews/Matchweek%201/4-1-8.png" alt="4.1" width="75%" />
  </p>

</details>

<details>
  <summary>Ladislav Krejčí</summary>

  - **Code**: [Ladislav-Krejčí.ipynb](./player-dashboard/CB/Ladislav-Krejčí.ipynb)  
  - **Summary**:
    It's been a fairly busy week on the transfer window for Wolves' standards, with the likes of Krejci and Uche having genuine agreements with both the club and the player, rather than being used as bait for bigger clubs (ahem, Pubill & Sanchez).

    With Krejci very close to signing with Wolves at 35m, many question whether it's worth the hefty price (Wolves usually sign 10m-20m players) and who he will replace. While most set out to find a backup LCB (like Renan), with Toti, Agbadou, and Doc/Mosquera as the [backline](./Project%202/Project%202.4/project2-4.ipynb). But with Krejci coming in, he surely is starting quality. I'm thinking Toti, Krejci, and Agbadou on the right. The interesting thing is, Wolves really are in need of such a progressive center back. Other than Doherty, there isn't really another one at the club, so I understand this sort of signing.

    Krejci has great distributions and if deployed on the left, I'm sure will pair very well with Hugo Bueno, who as I've mentioned, really impressed despite our [1-0 lost against Bournemouth yesterday](./match-reviews/Matchweek%202/8-23-2025.ipynb). His 96th percentile in progressive carrying distance really stands out for my case. Despite being a center back, he has more touches on average in the middle third (49.5%, or almost half) than defensive (46.7%). Therefore t's no suprise that he's a ball playing defender as well.

    However, he does lack a lot of defensive workrates. 4th percentile in passes blocked, 5th percentile in dribblers tackled, and 8th for tackles in general. That doesn't mean he don't make quality challenges, but it isn't frequent for a center back. Funny thing is, we did see it in full display today with his game against Villareal, with Tajon Buchanan scoring a hattrick and a 5 - 0 loss while having Krejci as the LCB in a back four.

  <p align="center">
    <img src="./player-dashboard/CB/Ladislav-Krejčí.png" alt="Ladislav Krejčí" width="75%" />
  </p>
</details>

<details>
  <summary>1.6 - Progressive Passes by Game State</summary>

  - **Code**: [project1_6.ipynb](./Project%201/Project%201.6/project1_6.ipynb)  
  - **Summary**:  
    Continuing on from previous progressive results, Joe from [Concept Scouting](https://x.com/ConceptScouting) suggested that I should look into game states (whether Wolves were ahead, level, or chasing) to determine "whether the PrgP is meaningful or just despirate". It's reasonable to say that Wolves are better to set up defensively and counter, rather than building out through repetitive progressions.

    For each game, we sum up the minutes Wolves were ahead, level, or behind in a game. We can plot this relationship over the course of the season. Progressive passes vs dominant game state (the state Wolves spent the most of the game in) reveals that less PrgP are made when the team is ahead, and more when behind. It makes sense to be more aggressive when trailing. Wolves are also towards the progressive end even when level in goals. We know this since the level median is closer to behind than ahead. It's also not a coincidence that the outliers themselves also reflect this trend.

    We can also plot minutes per game state. As expected, the more time spent ahead, the less PrgP, and more time spent behind, the more PrgP.

    I think I've been looking at this wrong. In the beginning of this project I thought Wolves were losing games because of high PrgP, possession, etc. Now I can confidently say that Wolves are making more PrgP because they're behind, and obviously more games are lost when more time was spent behind, which makes more sense.

    Unfortunately, this will mean the end of my first complete project.

  <p align="center">
    <img src="./Project%201/Project%201.6/1.6.png" alt="1.6" width="75%" />
  </p>
</details>




























## Match Reviews

- **Source(s)**: [FBref](https://fbref.com/en/squads/8cec06e1/Wolverhampton-Wanderers-Stats), [Sofascore](https://www.sofascore.com/team/football/wolverhampton/3), [Fotmob](https://www.fotmob.com/teams/8602/overview/wolverhampton-wanderers)
- **Folder**: [match-reviews](./match-reviews/)
- **Summary**: Recurring project to review previous games and key takeaways.

<details>
  <summary>(PL 25/26) BOU 1 - WOL 0</summary>

  - **Code**: [8-23-2025.ipynb](./match-reviews/Matchweek%202/8-23-2025.ipynb)  
  - **Summary**:
    The game could've ended much worse. With Toti being sent off early in the second half, it's interesting to see that Wolves played better with 10 men. However the substitutions made while trailing behind were questionable, subbing off Arias for Santiago Bueno to retain a back 3, but with limited attacking power when an equalizer is needed over defensive abilities. Perhaps Pereira wanted to push Hugo Bueno and Tchatchoua further up for crosses chances, which did occur, but lacked aggression as the game went on.

    It's sad to see the minimal amount of chances or creativity Wolves had, especially after taking Arias off. That being said, Hugo Bueno does look good with his crosses and progression. But why Agbadou taking the freekick and how Agbadou and Sa managed to bump into each other with zero pressure, I will never understand.

    Suprisingly, most of our shot creating actions came down the middle, which I feel is rare for Wolves.

  <p align="center">
    <img src="./match-reviews/Matchweek%202/4-2-5.png" alt="4.2" width="75%" />
  </p>

  I'm very suprised Bournemouth didn't score one or two more considering the insane amount of shot creating actions they had (51 v 22 for Wolves). A very left leaning attack consisting of Truffert, Brooks, and Semenyo compared to less pressure on the right. Which I'm guessing is why Hugo Bueno was able to push forward much more than Tchatchoua (who looked good today).

  We can also see large amounts of shots clustered in a small area, as well as a few threaded passes down the middle.

  <p align="center">
    <img src="./match-reviews/Matchweek%202/4-2-6.png" alt="4.2" width="75%" />
  </p>

  I believe Hugo Bueno and Tchatchoua should be our starting wing backs. Toti, Agbadou, and hopefully Mosquera on the right. Larsen up top, Arias to the left, then the right could be a mix of Rodrigo Gomes and Fer Lopez, who both have qualities that I feel are overlooked by the squad.

  <p align="center">
    <img src="./match-reviews/Matchweek%202/4-2-7.png" alt="4.2" width="75%" />
  </p>

  <p align="center">
    <img src="./match-reviews/Matchweek%202/4-2-8.png" alt="4.2" width="75%" />
  </p>

</details>

<details>
  <summary>(PL 24/25) BOU 0 - WOL 1</summary>

  - **Code**: [preMW2.ipynb](./match-reviews/Matchweek%202/preMW2.ipynb)  
  - **Summary**:
    With a 0-4 loss to City, Wolves are looking to bounce back against Bournemouth. Concerns for Agbadou and Jose Sa's form remains, but hopefully it will being to pick up. Bournemouth played Liverpool and Semenyo was the start of the show, scoring two goals from the right. It's no doubt the likes of KJH and Doc will have to put a shift in to stop that from happening. As a preview lets take a look at our last meeting against Bournemouth in the Premier League:

    The SCA map for Wolves reveals that our attack was mainly focused on the right, with 6 shots in the bottom half space. Bellegarde and Semedo (now KJH) driving up and providing support to the likes of Cunha and Munetsi. Compared to City, there was also way more build up play (74% 1/3 share v 90%). Hopefully KJH will be able to perform like last time against City, obviously with more quality crosses. I won't be suprised if Tchatchoua gets featured later in the game.

    The left hand side was fairly quiet that game. With Wolfe not making much of an impact against City, I'd like to see Hugo Bueno get more game time against Bournemouth. Perhaps Wolfe will perform better with a player like Arias in front of him, as mentioned by [@molineuxmusings](https://x.com/molineuxmusings/status/1957365672670896230). We could also potentially see Fer Lopez making creative player later in the game after Bellegarde subs off.

  <p align="center">
    <img src="./match-reviews/Matchweek%202/4-2-1.png" alt="4.2" width="75%" />
  </p>

  Bournemouth had no shortage of chances either. With Zabarnyi being shown a red early in the game, Bournemouth was lacking options in attack later in the game. Semenyo and Ouattara make a few good rights on the left against Doc, but the Wolves defence was able to hold it together. It's also important to note that they had a deeper build up play, favoring threaded passes or crosses past the halfway line, some of them even from Kepa. The likes of Toti, and Mosquera (should he start) will be pivotal in preventing the likes of Semenyo from progressing.

  <p align="center">
    <img src="./match-reviews/Matchweek%202/4-2-2.png" alt="4.2" width="75%" />
  </p>

  These maps really just confirm what I've just mentioned. Most of the shots from Wolves are concentrated towards the right, so are the crosses and dribbles. Bournemouth seemingly have actions all over the place. Both sides would really benefit from pacey players using the wider areas more.

  <p align="center">
    <img src="./match-reviews/Matchweek%202/4-2-3.png" alt="4.2" width="75%" />
  </p>

  <p align="center">
    <img src="./match-reviews/Matchweek%202/4-2-4.png" alt="4.2" width="75%" />
  </p>

</details>

<details>
  <summary>(PL 25/26) WOL 0 - MCI 4</summary>

  - **Code**: [postPatchweek1.ipynb](./match-reviews/Matchweek%201/postMatchweek1.ipynb)  
  - **Summary**:
    Despite the dissappointing 0-4 result, I believe it's revealing and there's a lot of new insights we can take from this game. Apart from a few major mistakes at the back, the team didn't look to bad imho.

    I'm suprised how central our attack was compared to last time we played city. A 48% centrality bias compared to last time's 13%. A few shots from Munetsi's offside as well as Larsen. Note that all these shows are clustered very close together as well. What impressed me however was Hoever, who not only dealt with Doku fairly well with Doherty (especially compared to last time) and made several progressive passes and crosses on the bottom wing of the graph. In fact, all 4 SCA crosses originated from the right side.
    
    Part of me wonders if there would've been better chances for Larsen if those crosses from the right were passes instead.

    What's concerning is the lack of progression from the left hand side / top wing. Wolfe and Bellegarde didn't contribute much to the attack. Neither did Hugo Bueno later on.

  <p align="center">
    <img src="./match-reviews/Matchweek%201/4-1-5.png" alt="4.1" width="75%" />
  </p>

  City also attacked fairly centrally, especially compared to last time. Obviously this is because of Haaland returning vs City playing KDB up top before. Fairly even distribution in passing. Less action on the left / top wing from Doku as mentioned. Much deeper build up play compared to us, but tbf that's what you expect from a team like City.

  <p align="center">
    <img src="./match-reviews/Matchweek%201/4-1-6.png" alt="4.1" width="75%" />
  </p>

  I mean the results speak for themselves on the plot below. Our options on the bench aren't bad either: Mosquera, Hugo Bueno, Rodrigo Gomes, Arias, Lopez, as well as Tchatchoua coming in soon. Hopefully it will only be up from here and both Agbadou & Sa gets in the right mindset.

  <p align="center">
    <img src="./match-reviews/Matchweek%201/4-1-7.png" alt="4.1" width="75%" />
  </p>

  <p align="center">
    <img src="./match-reviews/Matchweek%201/4-1-8.png" alt="4.1" width="75%" />
  </p>

</details>

<details>
  <summary>(PL 24/25) WOL 0 - MCI 1</summary>

  - **Code**: [matchweek1.ipynb](./match-reviews/Matchweek%201/matchweek1.ipynb)  
  - **Summary**:
    The first gameweek is coming up this weekend with a tough opponent to start of the season. Wolves only won 1 game against the top 6 last season (Villa). City was also the one to end our 6 game winstreak back in May, and we haven't won a single game since then. To be fair, the drop in form was after relegation is avoided and there's nothing to play for. 

    A good way to gauge this would be to look at our previous match up, which was a 1 - 0 defeat away at City. This first diagram shows us the lanes of attack Wolves where the most shot creating actions happened. Both the top and bottom half were frequent, with lack of central progressions (with the centrality bias being 13%).
    
    The most used attacking zone was the bottom half space of the final third, as circled and highlighted below, so I wouldn't be suprised if that space would be targeted once again. Ait Nouri's shot from the left (top half space) that hit the woodwork then a shot on target to follow up is noted as well. Obviously he playes for Man City now.

  <p align="center">
    <img src="./match-reviews/Matchweek%201/4-1-3.png" alt="4.1" width="75%" />
  </p>

  With City, our top half space defensively was heavily exploited. Doku's 13 progressive carries (next highest for City that game was 3), 5 shot creating actions, and 4/10 successful take ons allow him to dominate the left side. This would very likely happen again. Doesn't matter if KJH or Rodrigo Gomes, Wolves are pretty much cooked unless something crazy happens. City's 25% centrality bias perhaps influenced the only goal from De Bruyne. Both Doherty (or Mosquera) and Hoever (or Rodrigo Gomes) will have to put in a huge shift on Saturday to stop Doku (and Cherki, Marmoush, Foden, etc).  

  <p align="center">
    <img src="./match-reviews/Matchweek%201/4-1-4.png" alt="4.1" width="75%" />
  </p>

  Here at the bottom also shows the passes, dribbles, and crosses leading up to the shot itself. And the patterns in frequency reveals itself once again. I tried to use sofascore [here](./match-reviews/Matchweek%201/sofaScoreTest.ipynb) but couldn't figure out how to scale it properly after scraping so I just gave up. All these points I had to [click manually](https://fcpythonvideocoder.netlify.app/) from the highlights. 

  <p align="center">
    <img src="./match-reviews/Matchweek%201/4-1-1.png" alt="4.1" width="75%" />
  </p>

  <p align="center">
    <img src="./match-reviews/Matchweek%201/4-1-2.png" alt="4.1" width="75%" />
  </p>

</details>

## Player Dashboard

- **Source(s)**: [FBref](https://fbref.com/en/), [Sofascore](https://www.sofascore.com/), [Fotmob](https://www.fotmob.com/)
- **Folder**: [player-dashboard](./player-dashboard/)
- **Summary**: Recurring project to scout and analyze players with various metrics and visualizations.

<details>
  <summary>Tolu Arokodare</summary>

  - **Code**: [Tolu-Arokodare.ipynb](./player-dashboard/ST/Tolu-Arokodare.ipynb)  
  - **Summary**:
    With Uche's transfer seemingly being called off, Arokodare has been a focal point for the past few days. With a fee of around 20 to 25m with add ons, this could be a deal especially with Fabio Silva leaving for a similar amount. The eye test shows that Tolu has elite stats compared to many strikers. Things like shot and goal creating actions, expected goal involvements, and aerial wins. With him and JSL up front, with Hugo Bueno and Tchatchoua crossing in, and Arias providing threaded passes through the middle, there's no doubt that Wolves will be safe from relegation this season. With the likes of Kalajdzic, Lopez, Hwang, and Rodrigo Gomes as supersubs, there can be further chances later in the game

    One main concern is the amount of missed chances. Personally I think this is one of those things that we'll have to figure out when he plays.

  <p align="center">
    <img src="./player-dashboard/ST/Tolu-Arokodare.png" alt="Tolu Arokodare" width="75%" />
  </p>
</details>

<details>
  <summary>Ladislav Krejčí</summary>

  - **Code**: [Ladislav-Krejčí.ipynb](./player-dashboard/CB/Ladislav-Krejčí.ipynb)  
  - **Summary**:
    It's been a fairly busy week on the transfer window for Wolves' standards, with the likes of Krejci and Uche having genuine agreements with both the club and the player, rather than being used as bait for bigger clubs (ahem, Pubill & Sanchez).

    With Krejci very close to signing with Wolves at 35m, many question whether it's worth the hefty price (Wolves usually sign 10m-20m players) and who he will replace. While most set out to find a backup LCB (like Renan), with Toti, Agbadou, and Doc/Mosquera as the [backline](./Project%202/Project%202.4/project2-4.ipynb). But with Krejci coming in, he surely is starting quality. I'm thinking Toti, Krejci, and Agbadou on the right. The interesting thing is, Wolves really are in need of such a progressive center back. Other than Doherty, there isn't really another one at the club, so I understand this sort of signing.

    Krejci has great distributions and if deployed on the left, I'm sure will pair very well with Hugo Bueno, who as I've mentioned, really impressed despite our [1-0 lost against Bournemouth yesterday](./match-reviews/Matchweek%202/8-23-2025.ipynb). His 96th percentile in progressive carrying distance really stands out for my case. Despite being a center back, he has more touches on average in the middle third (49.5%, or almost half) than defensive (46.7%). Therefore t's no suprise that he's a ball playing defender as well.

    However, he does lack a lot of defensive workrates. 4th percentile in passes blocked, 5th percentile in dribblers tackled, and 8th for tackles in general. That doesn't mean he don't make quality challenges, but it isn't frequent for a center back. Funny thing is, we did see it in full display today with his game against Villareal, with Tajon Buchanan scoring a hattrick and a 5 - 0 loss while having Krejci as the LCB in a back four.

  <p align="center">
    <img src="./player-dashboard/CB/Ladislav-Krejčí.png" alt="Ladislav Krejčí" width="75%" />
  </p>
</details>










## 3 - Outlying Player Valuations

- **Source(s)**: [FBref](https://fbref.com/en/), [Transfermarkt](https://www.transfermarkt.com/)
- **Folder**: [Project 3](./Project%203/)
- **Summary**: Dedicated to finding outlying players across different leagues in various on field actions. For example, goal contributions by market value for strikers, wingers, or attacking midfielders. Then finding the best value per goal contribution. 

<details>
  <summary>3.1 - Striker Usage Rates</summary>

  - **Code**: [project3-1.ipynb](./Project%203/Project%203.1/project3-1.ipynb)  
  - **Summary**:
    Saw [this video](https://www.youtube.com/watch?v=iydcB3OM6EE) the other day and I got me thinking about Usage Rates. While it's mainly used in the NBA, usage rates are a great way to show how often a player gets the ball (whether or not they're the main man) and how efficient / productive they are with it. In football, this can be calculated by the sum of miscontrols, dispossessions, incomplete passes, failed take ons, and shots

    Some strikers get the ball a lot (like Cunha) and produce just as much results. Others get the ball a lot but doesn't convert them well, and so shouldn't really get the ball as much. There are also those that rarely get the ball, but makes it count whenever they do. In that case, they should be getting more of the ball, relative to the entire team.

    Just like in the video mentioned, I plotted the SCA and Usage Per 90 for all recent Wolves strikers. It's no suprise that Cunha is in the top right, and clearly deserving the volume of involvement he gets. Tolu impresses as well, seemingly having a similar trajectory as Cunha.

    On the other hand, those like Larsen, despite having both low usage and SCA, has high G+A, simply because he isn't that involved in the build up.

    What stands out however, is Willian Jose. While his stint at Wolves as a short term replacement for Jimenez wasn't too successful, the shot creating actions he was able to generate, considering his very low usage, is impressive. This makes him on par with the likes of Tolu and Cunha.

  <p align="center">
    <img src="./Project%203/Project%203.1/3-1-1.png" alt="3.1" width="75%" />
  </p>

  Now since this project is about player valuations, lets take a look at how well a player uses the ball with value. Once again we see Cunha having both high value and usage. Tolu has great usage considering his price range, so does Kalajdzic (who had just left to LASK on loan). Since price and usage don't grow at the same rate, naturally cheaper players will have the highest "value per million". But it's easier to see the ones that stand out by separating them by price range, as seen on the graphs below.

  <p align="center">
    <img src="./Project%203/Project%203.1/3-1-2.png" alt="3.2" width="75%" />
  </p>

</details>

## 2 - 2025 Summer Squad Assessment

- **Source(s)**: [FBref](https://fbref.com/en/squads/8cec06e1/2024-2025/Wolverhampton-Wanderers-Stats)
- **Folder**: [Project 2](./Project%202/)
- **Summary**: I've just finished the [3rd chapter of soccermatics](https://soccermatics.readthedocs.io/en/latest/lesson3/ScoutingPlayers.html) so it made sense for me to play around with the likes of radar plots & percentiles. This project will consist of developing a system to scout rumoured, linked, and new Wolves players for the upcoming season, comparing them to current or recently departed players.

<details>
  <summary>2.8 - Arokodare's Finishing Problem</summary>

  - **Code**: [stcomp.ipynb](./Project%202/Project%202.8/stcomp.ipynb)  
  - **Summary**:
  The other day while I was looking into [Arokodare](./player-dashboard/ST/Tolu-Arokodare.ipynb), I stumbled upon [this article](https://scoutedftbl.com/tolu-arokodare-goalscorer-cant-finish/). While on the surface his goals per 90 ratio is impressive, what's often overlook is how clinical he really is.

  Let's take Larsen as an example. In a Wolves team that lacks creativity and chances, he really don't get flooded with opportunities to shoot. It's expected that his non penalty goals are 0.35, but in reality he overperforms by a lot, scoring 0.45 non penalty goal per game. Since his npxG < npG, he's doing better than expected. On the other hand, despite Arokodare scoring more, his expected goals (0.81) is far greater than his actual goals per game (0.62). This means that he's underperforming. Considering the amount of shots he took, he should've scored way more. Granted, Tolu Arokodare was given an insane amount of chances, basically with over 7.4 progressive passing receptions at Genk compared to 4.06 with Larsen.

  I'm a little worried that Wolves being not as progressive as Genk will mean that Tolu will suffer from the lack of opportunities, and when he does get them, have a much bigger chance of being less clinical than he should be.

  <p align="center">
    <img src="./Project%202/Project%202.8/2-8-1.png" alt="2.8" width="75%" />
  </p>

  Let's also take a look at Arokodare's number of shots per game, which is nearly 5 per 90. 32.7% of them are on target, and 12.4% of them are goals. On the other hand, Larsen has 60.7% shots on target and 23% of shots turn into goals. The numbers are quite telling when you put it out like that.

  <p align="center">
    <img src="./Project%202/Project%202.8/2-8-2.png" alt="2.8" width="75%" />
  </p>

  Interestingly enough, there's actually a correlation to this. [@ctwwfc](https://x.com/ctwwfc) suggested that the inflated amounts of shots could be related to the much higher goals prevented for GKs specifically in the Belgian league, as mentioned [on this post](https://x.com/wakocd_/status/1958854878572220442?s=46&t=53TKqHBsknak6IXfcVhk2g).
  
  Lammens, who had just transferred to United, is one of those keepers, who has an unusually high goals prevented at 15.57 last season. While its easy for many to compare stats to the likes of Onana, its important to note that the difficulty of shots are often not accounted for in different leauges (Onana back in Ajax had similar numbers). So it's no doubt that Lammens' numbers will drop off at United.

  Despite the high number of saves per 90, [Tolu actually scored a brace against him end of last year](https://fbref.com/en/matches/b4ea65cc/Antwerp-Genk-December-26-2024-Belgian-Pro-League). Arokodare registered 9 shots that game, 5 of them on target, and scoring 2. Lammens on the other hand faced 11 shots on target against (5 from Tolu) and conceding the only 2 against Tolu. The 81.8 save% is impressive, but is also a prime example of Tolu performing below his xG. The game ended 2-2, with Genk having an xG of 3.1.

  Interested to see how Tolu and Lammens' numbers will pan out throughout the season, especially in the prem. Despite being in different positions, it's no question that the data draws parallel with one another. However it's no doubt that their numbers will drop. Tolu will have to be much more clinical than what he is now if he wants to make it in the prem.

  <p align="center">
    <img src="./Project%202/Project%202.8/2-8-3.png" alt="2.8" width="75%" />
  </p>

  With the transfer window being closed, this marks the end of project 2 as well. Future rumors and links, new players and those of interest, will be broken down under the [Player Dashboard](#player-dashboard), which will be continuously updated, similar to the [Match Reviews](#match-reviews). For my next project I'm going full moneyball and finding overlooked / outlying players based on different in game metrics.

</details>

<details>
  <summary>2.7 - Bentley over Sa?</summary>

  - **Code**: [project2-7.ipynb](./Project%202/Project%202.7/project2-7.ipynb)  
  - **Summary**:
    Like Agbadou, Sa had an abysmal performance against City. Basically unable to save any shots on target that game. Many argued that Sa might be currently the worst keeper in the Prem, suggested that even Bentley should start over him.

    The stats don't lie either: 43% of shots on target turn into goals when Sa is playing. Granted, Sa has fairly difficult shots to face, but his save percentage is way below average and is definitely underperforming. Johnstone isn't any better either. Not only have he been facing much easier shows, his save % is just about the same. Bentley really stands out from the three. Granted, these stats are from the championship, but who knows what kind of performances he's able to bring?

    Only 38% of shots on target turn into goals, much more difficult shots, and higher save %. Granted he's not a sweeper, but is underperforming less than the likes of Sa and Johnstone. Interested to see if he gets a chance in between the sticks this season.

  <p align="center">
    <img src="./Project%202/Project%202.7/2-7-1.png" alt="2.7" width="75%" />
  </p>

</details>

<details>
  <summary>2.6 - Beyond Larsen</summary>

  - **Code**: [project2-6.ipynb](./Project%202/Project%202.6/project2-6.ipynb)  
  - **Summary**:
    Despite just signing for Wolves, Larsen is already being pursuited by the likes of Newcastle. It's no doubt that he (along with Andre and Joao Gomes) will be staying for long after this season.

    There are a also links with Uche at Getafe, who I believe will pair well with Larsen. He is able to do will in areas Larsen can't: Progressive Actions, Take Ons, Touches in the Pen, and Shot Creating Actions.

  <p align="center">
    <img src="./Project%202/Project%202.6/2-6-1.png" alt="2.6" width="75%" />
  </p>

  Of course, Larsen's goals per shot ratio is way above average. 60% of his shots are on target. 25% of his shots are goals. This means he scores every 4 shots he makes. This ratio is better than Haaland btw (I think hes around 21%).

  To be honest, the likes of Kalajdzic and Silva are both overlooked as well. Who knows how well they will play when they get a chance.

  <p align="center">
    <img src="./Project%202/Project%202.6/2-6-2.png" alt="2.6" width="75%" />
  </p>

</details>

<details>
  <summary>2.5 - New Wing Back Choices</summary>

  - **Code**: [tchatchoua.ipynb](./Project%202/Project%202.5/tchatchoua.ipynb)  
  - **Summary**:
    With new wing back signings Tchatchoua and Wolfe, lets revisit their metrics with different situations.

    Many argue that Tchatchoua has lacking qualities other than speed because his stats a underwhelming to say the leastt. On the other hand, what he excels on covers what Hoever is missing. Both 82nd %tile in Take on Success and 71st %tile in % Defensive Third Tackles reflects that he is great a 1 on 1 play (both with or without the ball), which is something Pereira admires. His frequency of progressive actions is also solid: 4.34 touches on average per PrgA.

  <p align="center">
    <img src="./Project%202/Project%202.5/2-5-1.png" alt="2.5" width="75%" />
  </p>

  Hoever (KJH) on the other hand is more defensively sound that most people think. Suprisingly, his actions in the middle third (37.43%) is nearly just as much as his defensive third (39.97%). He also has a high attacking ratio for a wing back at 24.64%. Ultimately, he has a better chance of a shot creating action by passing rather than crossing. The good thing is that we saw all these qualities in the recent City game, as mentioned in the [matchweek 1 review](./match-reviews/Matchweek%201/postMatchweek1.ipynb).

  <p align="center">
    <img src="./Project%202/Project%202.5/2-5-2.png" alt="2.5" width="75%" />
  </p>

  Wolfe is interesting because he had a mediocure game against City. But his 98th percentile for dribblers tackled is often overlooked. Good amount of touches in the pen, and is solid in goal creations. Interesting to see that he made no crosses into the penalty box in the last 365 days, and lacking carries (23% compared to Hugo Buenos 60%).

  <p align="center">
    <img src="./Project%202/Project%202.5/2-5-3.png" alt="2.5" width="75%" />
  </p>

  Lastly, Bueno arguably has better progression than Wolfe. 96th percentile on take on success and the best of all Wolves WBs in terms of touches per progressive actions. Also very high quality actions into the penalty box, so every pass, cross, and carry into the penalty box has a very high chance to turning into a shot creating action.

  <p align="center">
    <img src="./Project%202/Project%202.5/2-5-4.png" alt="2.5" width="75%" />
  </p>

  Just realised I completely forgot about Rodrigo Gomes after his goal against West Ham in the FA cup yesterday. Despite being a very attackiong wingback, maybe even a winger, his defensive attributes are still solid. With 6.76 touches per defensive action (best of all wing backs here), it's also complemented by his progression. 3.47 touches per progressive actions and 2.33 touches per attacking third touch means that a good chunk of his actions are further up the pitch. 40.24% in the middle third backs it up. I loved his efforts in yesterdays game, where he even scored a rebound off Hwang's missed penalty. He will be crutial in cup games and as a supersub scoring / assisting equalizers / winners later in the game this season for sure.

  <p align="center">
    <img src="./Project%202/Project%202.5/2-5-5.png" alt="2.5" width="75%" />
  </p>

Overall I would say Hugo Bueno and Tchatchoua should be starting wingbacks. I really like Bueno's progression and how aggressive he is. Despite Tchatchoua's below par stats, the energy he injects to the game provides much needed pace for the team.

  <p align="center">
    <img src="./Project%202/Project%202.5/2-5-6.png" alt="2.5" width="75%" />
  </p>

</details>

<details>
  <summary>2.4 - CB Depth Situation</summary>

  - **Code**: [project2-4.ipynb](./Project%202/Project%202.4/project2-4.ipynb)  
  - **Summary**:
    The starting center back roles are primarily sorted. But then comes the issue of squad depth. It's no suprise the backline to start the season would likely consist of Toti, Agbadou, and Doherty, with Mosquera slowly implemented back into the squad, mainly use to his shaky injury record. That said, we are one injury away from a defensive crisis. With only Santiago Bueno as backup, there isn't anyone else to fill that LCB position if Toti gets injured.

    Renan, Disasi, and Kelly are among the few players linked to this role. Both Disasi and Kelly are out of favor in their respective clubs. Disasi is a potential option with Wolves considering a deal with him and striker Fofana. Kelly is another fair choice, with high defensive work rates as well as progressive distributions. However with his wage being upwards of 80k I don't see this happening. This leaves us with Renan, who has some of the best ball distribution stats of the bunch.

  <p align="center">
    <img src="./Project%202/Project%202.4/2-4-1.png" alt="2.4" width="75%" />
  </p>

  Lets focus on Renan: 4.1 tackles and interceptions, 4.7 recoveries, 7.1 progressive actions and 5 final third entries (all per 90). Granted this was during his time at Internacional last year, but the point still stands. It's also important to mention Toti's impressive 1.05 OF - xOF, which stands for the difference between his on off goal difference and expected on off goal difference. He not only has a positive xOF, but exceeds that threshold when on the pitch.

  <p align="center">
    <img src="./Project%202/Project%202.4/2-4-2.png" alt="2.4" width="75%" />
  </p>

  And it shows here too, with Toti having the best team impact score of all sampled players. The only progressive player currently is Doherty, so higher progression is always welcomed in wider center back roles, such as Renan and Disasi.

  <p align="center">
    <img src="./Project%202/Project%202.4/2-4-3.png" alt="2.4" width="75%" />
  </p>

  Below are further metrics and distributions of all the players referenced and used for comparison. You can see how the wide backs are more progressive than the center backs (Agbadou), hence in search of a LCB the focus is a little more towards ball distribution, making Renan a great candidate.

  <p align="center">
    <img src="./Project%202/Project%202.4/2-4-4.png" alt="2.4" width="75%" />
  </p>

</details>

<details>
  <summary>2.3 - Replacing Cunha</summary>

  - **Code**: [project2-3.ipynb](./Project%202/Project%202.3/project2-3.ipynb)  
  - **Summary**:  
    With Cunha leaving to United, I'm interested to see how Wolves will replace the 62.5m euro man. And realistically, his stats won't be replicated at Wolves for a while. Out of all 10 categories, when compared to departing, current, and rumored Wolves players (12), Cunha tops 4 of them, and is 3rd in two others. With a +6.4 difference in non penalty goals and expected goals, the next closest of the bunch is Akturkoglu with +1.3, who stands out as one of the best replacements, and would play well along side the likes of Arias and Lopez. As seen below, he also has the most podium finishes after Cunha.

  <p align="center">
    <img src="./Project%202/Project%202.3/2-3-1.png" alt="2.3" width="75%" />
  </p>

  We can highlight these players (another good pick would be Ben Doak) and split them by shooting, progression, and pressing. It's easy to notice the similarities between Matheus and Kerem. Identical expected goal contributions and shots on target per 90, similar progressively and both fairly aggressive. Despite his lower take ons and npG-xG, Kerem makes up for in touches in the opposite pen and interceptions. Again Ben Doak shares similar stats in the Championship last season. I believe these two are arguably better picks than the likes of Amine Adli and Matthis Abline, both who are more popular choices. 

  <p align="center">
    <img src="./Project%202/Project%202.3/2-3-2.png" alt="2.3" width="75%" />
  </p>

  Here Cunha and Akturkoglu both are the only shot dominant players, which is something we're lacking after Cunha imo. Bellegarde and Munetsi provide depth to both midfield and CAM, hence their press heavy characteristics, espeically for attacking players. Progressive architypes are pretty common, since Wolves already have Arias and Lopez, but Doak would be a good addition as well. Adli and Abline are good too but I would personally perfer Kerem and Ben. That way, Wolves would have a Cunha like player and sufficient progressive options (as well as press heavy like Munetsi).

  <p align="center">
    <img src="./Project%202/Project%202.3/2-3-3.png" alt="2.3" width="75%" />
  </p>

  Below are further metrics and distributions of all the players referenced and used for comparison.

  <p align="center">
    <img src="./Project%202/Project%202.3/2-3-4.png" alt="2.3" width="75%" />
  </p>

</details>

<details>
  <summary>2.2 - RWBs Lacking Quality</summary>

  - **Code**: [project2-2.ipynb](./Project%202/Project%202.2/project2-2.ipynb)  
  - **Summary**:  
    This is probably one of the most detailed sub projects so far and was a pain to code out.

    There's currently a dilemma for the right wing back (RWB) position at Wolves. Like Ait Nouri, Semedo had just left and there are large shoes to fill once again. Other options are Hoever (KJH), who just like Hugo Bueno in 2.1 just returned from loan (Auxerre). On the other hand with Rodrigo Gomes who had a few good rotational minutes, scoring in both games against Leicester. Pedro Lima has potential but with limited minutes he could be going out on loan.

    Many think KJH and R. Gomes aren't exactly premier league proven, and Wolves have been searching for an established wing back. Almost aquiring Pubill (who played with Hugo Bueno recently at the U21 Euros), however the deal was hijacked last minute by Athletico. Another rumor that stands out would be Sanchez (also played with both at U21 Euros), who as of writing is reluctant to sign for Wolves for the same reason: lack of European football and ambition.

    It's no suprise that their agents are using Wolves as a chip to lure other more ambitious clubs to sign. And it's also no suprise that KJH would get the starting role against City this weekend. We can compare the departed, current, and rumored players in a donut bar chart to see the overall trend / type of RWB Wolves tend to prefer.

  <p align="center">
    <img src="./Project%202/Project%202.2/2-2-1.png" alt="2.2" width="75%" />
  </p>
  
  We split the donut into offensive and defensive attributes. Each player is compared to another and naturally higher numbers float towards the edge. In the rank grid to the right, we can see how Ratiu and Sanchez have some of the best stats. Ratiu is top for shot creating actions and successful take ons, both as I've mentioned in 2.1 are crutial to Pereira's play style. On the other hand, Sanchez tops in tackles, interceptions, blocks, and expected goal contributions. Ratiu also finishes top in the podium, with 2 1st place finishes and 5 2nd / 3rd finishes.

  <p align="center">
    <img src="./Project%202/Project%202.2/2-2-2.png" alt="2.2" width="75%" />
  </p>

  The individual player donuts also show the same thing. I think R. Gomes would be a phenominal rotational / supersub player this season, turning tackles / interceptions into progressive actions later in the game. You can also see some of the weakesses Ratiu or even KJH would be able to cover up with Semedo now gone.

  <p align="center">
    <img src="./Project%202/Project%202.2/2-2-3.png" alt="2.2" width="75%" />
  </p>

  Below are further metrics and distributions that I thought could add to this project.

  <p align="center">
    <img src="./Project%202/Project%202.2/2-2-4.png" alt="2.2" width="75%" />
  </p>

</details>

<details>
  <summary>2.1 - Wolfe or Bueno?</summary>

  - **Code**: [project2-1.ipynb](./Project%202/Project%202.1/project2-1.ipynb)  
  - **Summary**:  
    With Ait Nouri leaving the Man City in the beginning of the window, there were big shoes to fill on the left wing back position. Hugo Bueno, who is homegrown and had just returned from a fairly decent loan under Van Persie at Feyenoord, was expected to step up. Wolfe was also signed from Alkmaar, and it looks like they will share minutes for the spot as of now.

    The basic radar plot generated can be split in half for the LWB's offensive and defensive attributes. For instant, Progressive actions are a sum of progressive carries, passes, and receptions. These are scaled and normalized to the selection of players in question, so for example Ait Nouri (RAN) seems to have 100% Successful Take Ons but that's because he has the most of the three.

    It's easy to notice why RAN was so successful under Pereira. As [Doherty mentioned in an interview](https://www.youtube.com/watch?v=ZbGNFc41OlU&ab_channel=Wolves), Pereira prefers wing backs to take on opponents 1v1 rather than passing with support (like Nuno). I'm expecting Bueno to start the first game against City, but interested to see what happens beyond that.

  <p align="center">
    <img src="./Project%202/Project%202.1/2-1.png" alt="2.1" width="75%" />
  </p>

</details>

## 1 - Progression Analysis (24/25)
<!-- **1 - Wolverhampton Wanderers Analysis (24/25 Season)** -->

- **Source(s)**: [FBref](https://fbref.com/en/squads/8cec06e1/2024-2025/Wolverhampton-Wanderers-Stats)
- **Folder**: [Project 1](./Project%201/)
- **Summary**: For my first project and being a fan I decided to analyse data from Wolves. I was already familiar with the squad and its problems so this was a natural starting point.

<details>
  <summary>1.6 - Progressive Passes by Game State</summary>

  - **Code**: [project1_6.ipynb](./Project%201/Project%201.6/project1_6.ipynb)  
  - **Summary**:  
    Continuing on from previous progressive results, Joe from [Concept Scouting](https://x.com/ConceptScouting) suggested that I should look into game states (whether Wolves were ahead, level, or chasing) to determine "whether the PrgP is meaningful or just despirate". It's reasonable to say that Wolves are better to set up defensively and counter, rather than building out through repetitive progressions.

    For each game, we sum up the minutes Wolves were ahead, level, or behind in a game. We can plot this relationship over the course of the season. Progressive passes vs dominant game state (the state Wolves spent the most of the game in) reveals that less PrgP are made when the team is ahead, and more when behind. It makes sense to be more aggressive when trailing. Wolves are also towards the progressive end even when level in goals. We know this since the level median is closer to behind than ahead. It's also not a coincidence that the outliers themselves also reflect this trend.

    We can also plot minutes per game state. As expected, the more time spent ahead, the less PrgP, and more time spent behind, the more PrgP.

    I think I've been looking at this wrong. In the beginning of this project I thought Wolves were losing games because of high PrgP, possession, etc. Now I can confidently say that Wolves are making more PrgP because they're behind, and obviously more games are lost when more time was spent behind, which makes more sense.

    Unfortunately, this will mean the end of my first complete project.

  <p align="center">
    <img src="./Project%201/Project%201.6/1.6.png" alt="1.6" width="75%" />
  </p>

</details>

<details>
  <summary>1.5 - Possession vs. Goal Difference (Bottom 14 & Manager)</summary>

  - **Code**: [project1_5.ipynb](./Project%201/Project%201.5/project1_5.ipynb)  
  - **Summary**:  
    Drawing inspiration from previous progressive results, and [Soccermatic's possession samples](https://soccermatics.readthedocs.io/en/latest/lesson2/Possession.html), I plotted such relationships by filtering out top 6 teams (where progressiveness didn't matter) and noticed the following trends:

    - No obvious relationship between possession and goal different when all games are plotted.
    - However when games against the top 6 are filtered out, data reveals that lower possession (and logically, progression) is related to positive goal difference, even for both Gary O'Neil and Vitor Pereira.
    - As an example, O'Neil was winless in games with 54%+ possession, which made up the bulk of his losses (against the bottom 14).
    - Pereira was unbeaten in games with <54% possession, which also made up the bulk of his wins (against the bottom 14).
    - Again, the only wins O'Neil had only game from the games with 54%+ possession.
    - On the flip side, all of Pereira's losses against the bottom 14 originated from games with <54% possession.

    All this provides valuable insights to concerns in progression as mentioned in 1.1 and 1.2, with possession backing up the correlation. Evidently, less progressive passes are able to be made if there's less possession of the ball, for obvious reasons. I'm interested to see if Pereira will still decide to play high possession and high progressiveness against bottom 14 teams, despite the negative results in that department.

    Based on [this video from Tifo Football](https://x.com/TifoFootball_/status/1702577998421987506) at 6:35 via [Jake Kolliari](https://x.com/_JKDS_), non penalty xG difference is one of the biggest indicators in avoiding relegation. Lucky for me, Wolves never won a single penalty so whether the plots included penalties or not makes no difference.
    
    I'm very confident that with low possession and lower amounts of (but higher quality) progressiveness against the bottom 14, most of these games are very winnable. If Wolves were to do that 24/25, European football would have very much been achievable, let alone surviving relegation.

  <p align="center">
    <img src="./Project%201/Project%201.5/1.5.png" alt="1.5" width="75%" />
  </p>

</details>

<details>
  <summary>1.4 - Scouted Player Progressions</summary>

  - **Code**: [project1_4.ipynb](./Project%201/Project%201.4/project1_4.ipynb)  
  - **Summary**:  
    A look into scouted / players linked with Wolves may give us a better idea of where Wolves may be heading in terms of progression next season. I used [@jay_wwfc07's scouted list](https://x.com/jay_wwfc07/status/1949467837384597551) on twitter as reference.

    - Milan Van Ewijk from Coventry have similar progressive profiles as RAN, and Rodrigo Gomes, so does Blas with Cunha.
    - Adli has high progressive carries, which is needed if Wolves decide to continue with high PrgP games. Which I still don't understand.

  <p align="center">
    <img src="./Project%201/Project%201.4/1.4.png" alt="1.4" width="75%" />
  </p>

</details>

<details>
  <summary>1.3 - Player Progressive Carries, Passes, and Receptions</summary>

  - **Code**: [project1_3.ipynb](./Project%201/Project%201.3/project1_3.ipynb)
  - **Summary**:  
    To understand the correlation with progression and recent results from 1.1 and 2, in 1.3 I looked into each player's contribution to progression.
    
    - When plotted against minutes played, starters like Cunha (Sold), RAN (Sold), Gomes, Semedo (Left) all stood out.
    - Interesting results came from PrgC, PrgP, and PrgR per 90. When plotted, supersubs / rotational players like R. Games, Sarabia (Left), Guedes (Sold), and Hwang outperformed the starters.
    - It's clear that Pereira uses these players later in the game for higher progression, but on the flip side cause more turnovers, which could explain some of the games lost.

  <p align="center">
    <img src="./Project%201/Project%201.3/1.3.png" alt="1.3" width="75%" />
  </p>

</details>

<details>
  <summary>1.2 - Match Outcomes vs. PrgP (By Manager), Final Third Passes, Crosses, Passing Distance</summary>

  - **Code**: [project1_2.ipynb](./Project%201/Project%201.2/project1_2.ipynb)
  - **Summary**:   Reached out to [Matt Penn](https://www.linkedin.com/in/matthew-penn-732551232/) for some help, who is an insights data scientist at the FA. He mentioned that it could be due to a change in managers. I looked into this, but it didn't matter whether it was GON or VP:
    
    - Both managers were winless in games with 32+ PrgP (which makes sense because Wolves were winless in all 17 in games with 32+ PrgP anyways in 1.1)
    - Pereira won 10 out of 13, all games with 31≥ PrgP
  
    Same thing with final third passes, crosses, and passing distance, where more of those correlated to more losses. Those results are at the bottom of the 1.2 code file.

  <p align="center">
    <img src="./Project%201/Project%201.2/1.2.png" alt="1.2" width="75%" />
  </p>

</details>

<details>
  <summary>1.1 - Match Outcomes vs. Progressive Passes (By Tier)</summary>
   
  - **Code**: [project1_1.ipynb](./Project%201/Project%201.1/project1_1.ipynb)
  - **Summary**: A lot of the games were lost due to progression. Maybe even too much of it:
  
    - Winless in all 17 in games with 32+ PrgP
    - 12 wins in 21 in games with 31≥ PrgP
    - Undefeated in all 12 games against the bottom 14, in games with ≤31 PrgP
    
    This doesn't really make much sense. More progression typically don't 
    correlate to less wins, but the data shows otherwise.

  <p align="center">
    <img src="./Project%201/Project%201.1/1.1.png" alt="1.1" width="75%" />
  </p>

</details>