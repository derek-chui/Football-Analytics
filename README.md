# Football-Analytics

In this repository all the projects, as well as the tools resources that helped me create analysis & visualisation of football (soccer) data. Commonly used tools and software include Python, Web Scraping, NumPy, Pandas, Matplotlib, Seaborn, and Jupyter Notebook. Click on the arrow to select a project to expand for more details!

## Projects

**1 - Analytics on Wolverhampton Wanderers in the Premier League ahead of the 25/26 season**

<details>
  <summary>1.1 - Match Outcomes vs. Progressive Passes (By Tier)</summary>
  
  - **Sources**: [FBref](https://fbref.com/en/squads/8cec06e1/2024-2025/matchlogs/c9/passing/Wolverhampton-Wanderers-Match-Logs-Premier-League)  
  - **Code**: [`project1_1.ipynb`](./Project%201/Project%201.1/project1_1.ipynb)
  - **Summary**:  
    For my first project and being a fan I decided to analyse data from Wolves. Here was the first thing I notice right off the bat:
    - Winless in all 17 in games with 32+ PrgP
    - 12 wins in 21 in games with 31≥ PrgP
    - Undefeated in all 12 games against the bottom 14, in games with ≤31 PrgP
  
    This doesn't really make much sense. More progression typically don't correlate to less wins, but the data shows otherwise.

  <img width="2500" height="1409" alt="image" src="https://github.com/user-attachments/assets/48930d95-b9ab-42ad-a1f4-72754aacda12" />

</details>

<details>
  <summary>1.2 - Match Outcomes vs. PrgP (By Manager), Final Third Passes, Crosses, Passing Distance</summary>
  
  - **Sources**: [FBref](https://fbref.com/en/squads/8cec06e1/2024-2025/matchlogs/c9/passing/Wolverhampton-Wanderers-Match-Logs-Premier-League), [FBref](https://fbref.com/en/squads/8cec06e1/2024-2025/matchlogs/c9/misc/Wolverhampton-Wanderers-Match-Logs-Premier-League)
  - **Code**: [`project1_2.ipynb`](./Project%201/Project%201.2/project1_2.ipynb)
  - **Summary**:  
    Reached out to Matt Penn for some help, who is an insights data scientist at the FA. He mentioned that it could be due to a change in managers. I looked into this, but it didn't matter whether it was GON or VP:
  
    - Both managers were winless in games with 32+ PrgP
    - Pereira won 10 out of 13, all games with 31≥ PrgP
  
    Same thing with final third passes, crosses, and passing distance, where more of those correlated to more losses.

</details>

<details>
  <summary>1.3 - Player Progressive Carries, Passes, and Receptions</summary>
  
  - **Sources**: [FBref](https://fbref.com/en/squads/8cec06e1/Wolverhampton-Wanderers-Stats)  
  - **Code**: [`project1_3.ipynb`](./Project%201/Project%201.3/project1_3.ipynb)
  - **Summary**:  
    To understand the correlation with progression and recent results from 1.1 and 2, in 1.3 I looked into each player's contribution to progression.
    - When plotted against minutes played, starters like Cunha (Sold), RAN (Sold), Gomes, Semedo (Left) all stood out.
    - Interesting results came from PrgC, PrgP, and PrgR per 90. When plotted, supersubs / rotational players like R. Games, Sarabia (Left), Guedes (Sold), and Hwang outperformed the starters.
    - It's clear that Pereira uses these players later in the game for higher progression, but on the flip side cause more turnovers, which could explain some of the games lost.

<img width="2500" height="1409" alt="image" src="https://github.com/user-attachments/assets/680d2982-28e0-417b-b152-3b3936e5d892" />

</details>

<details>
  <summary>1.4 - Scouted Player Progressions</summary>
  
  - **Sources**: [FBref](https://fbref.com/en/squads/8cec06e1/Wolverhampton-Wanderers-Stats), [Twitter](https://x.com/jay_wwfc07/status/1949467837384597551)
  - **Code**: [`project1_4.ipynb`](./Project%201/Project%201.4/project1_4.ipynb)  
  - **Summary**:  
    A look into scouted / players linked with Wolves may give us a better idea of where Wolves may be heading in terms of progression next season. I used [@jay_wwfc07's scouted list](https://x.com/jay_wwfc07/status/1949467837384597551) on twitter as reference.
    - Milan Van Ewijk from Coventry have similar progressive profiles as RAN (Sold), and Rodrigo Gomes, so does Blas with Cunha.
    - Adli has high progressive carries, which is needed if Wolves decide to continue with high PrgP games. Which I still don't understand.

<img width="2500" height="1409" alt="image" src="https://github.com/user-attachments/assets/fc6cca8c-7959-42a0-a7cf-34fdb7b1d7de" />

</details>
