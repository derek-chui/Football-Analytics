# Football Analytics

This repo contains the projects, tools, and resources for football data analysis & visualisation. Commonly used tools include Python, Web Scraping, NumPy, Pandas, Matplotlib, Seaborn, and Jupyter Notebook. Several visuals from various projects can also be found on Twitter ([@thatderekchui](https://x.com/thatderekchui)).

Click on the arrows to select and expand each project for more details!

## 2 - Wolverhampton Wanderers Scouting (25/26 Season)

- **Source(s)**: [FBref](https://fbref.com/en/squads/8cec06e1/2024-2025/Wolverhampton-Wanderers-Stats)
- **Folder**: [Project 2](./Project%202/)
- **Summary**: I've just finished the [3rd chapter of soccermatics](https://soccermatics.readthedocs.io/en/latest/lesson3/ScoutingPlayers.html) so it made sense for me to play around with the likes of radar plots & percentiles. This project will consist of developing a system to scout rumoured, linked, and new Wolves players for the upcoming season, comparing them to current or recently departed players.

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

  Below are further metrics and distributions of all the players referenced and used for comparison. You can see ho the wide backs are more progressive than the center backs (Agbadou), hence in search of a LCB the focus is a little more towards ball distribution, making Renan a great candidate.

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

## 1 - Wolverhampton Wanderers Analysis (24/25 Season)
<!-- **1 - Wolverhampton Wanderers Analysis (24/25 Season)** -->

- **Source(s)**: [FBref](https://fbref.com/en/squads/8cec06e1/2024-2025/Wolverhampton-Wanderers-Stats)
- **Folder**: [Project 1](./Project%201/)
- **Summary**: For my first project and being a fan I decided to analyse data from Wolves. I was already familiar with the squad and its problems so this was a natural starting point.

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