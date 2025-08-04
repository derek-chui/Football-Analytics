# Football Analytics

This repo contains the projects, tools, and resources for football data analysis & visualisation. Commonly used tools include Python, Web Scraping, NumPy, Pandas, Matplotlib, Seaborn, and Jupyter Notebook. Several visuals from various projects can also be found on Twitter ([@thatderekchui](https://x.com/thatderekchui)).

Click on the arrows to select and expand each project for more details!

## Projects

**1 - Wolverhampton Wanderers Analysis (24/25 Season)**

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
  <summary>1.5 - Posession vs. Goal Difference (Bottom 14 & Manager)</summary>

  - **Code**: [project1_5.ipynb](./Project%201/Project%201.5/project1_5.ipynb)  
  - **Summary**:  
    Inspired by previous progressive results, and [Soccermatic's possession samples](https://soccermatics.readthedocs.io/en/latest/lesson2/Possession.html), I plotted such relationships by filtering out top 6 teams (where progressiveness didn't matter) and noticed the following trends:

    - No obvious relationship between possession and goal different when all games are plotted.
    - However when games against the top 6 are filtered out, data reveals that lower possession (and logically, progression) is related to positive goal difference, even for both Gary O'Neil and Vitor Pereira.
    - As an example, O'Neil was winless in games with 54%+ possession, which made up the bulk of his losses (against the bottom 14).
    - Pereira was unbeaten in games with <54% possession, which also made up the bulk of his wins (against the bottom 14).
    - Again, the only wins O'Neil had only game from the games with 54%+ possession.
    - On the flip side, all of Pereira's losses against the bottom 14 originated from games with <54% possession.

    All this provides valuable insights to concerns in progression as mentioned in 1.1 and 1.2, with possession backing up the correlation. Evidently, less progressive passes are able to be made if there's less possession of the ball, for obvious reasons. I'm interested to see if Pereira will still decide to play high possession and high progressiveness against bottom 14 teams, despite the negative results in that department.
    
    I'm very confident that with low possession and lower amounts of (but higher quality) progressiveness against the bottom 14, most of these games are very winnable. If Wolves were to do that 24/25, European football would have very much been achievable, let alone surviving relegation.

  <p align="center">
    <img src="./Project%201/Project%201.5/1.5.png" alt="1.5" width="75%" />
  </p>

</details>