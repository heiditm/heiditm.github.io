# VGChartz Video Game Sales EDA

Here we will explore the  [**VGChartz Video Game Sales**](https://www.kaggle.com/datasets/sidtwr/videogames-sales-dataset?resource=download&select=Video_Games_Sales_as_at_22_Dec_2016.csv) dataset through exploratory data analysis (EDA), an interactive dashboard (Tableau) and predictive analysis (Classification).

**Time Frame Conducted:** 1980 - 2020   
**Source:** Kaggle  

**Synopsis of Study:** VGChartz is a network consisting of 5 video game websites: VGChartz, gamrFeed, gamrReview, gamrTV and gamrConnect. The platform provides weekly game sales tracking by region along with tools for data analysis and reviews for the video gaming industry. The dataset used for this project consist of sales and review data for different platform and games between the years listed above.

This dataset consists of 16,719 observations and 16 variables:
- Completed Cases: 6,825

Variable|Description
-|:---
Name|Name of the game
Platform|Platform of the game
Year of Release|Year the game was released
Genre|Genre of the Game
Publisher|Publisher of the Game
NA|Sales in North America (in Millions)
EU|Sales in Europe (in Millions)
JP|Sales in Japan (in Millions)
Other|Sales in rest of the world (in Millions)
Global|Total worldwide sales (in Millions)
Critic Score|Aggregate score compiled by Metacritic staff
Critic Count|Number of Critics that gave a score
User Score|Score by Metacritic's subscribers
User Count|Number of Users (Metacritic's subscribers) that gave a score
Developer|Developer of the game
Rating|Entertainment Software Rating Board (ESRB) Rating of the Game
Type|Handheld or Console based on type of Platform

## Platform

There are a lot of platforms in this dataset which are all written in acronyms. This table shows their full names, this helped me a lot and I hope it helped you too!

Platform|Description
-|:---
2600|Atari 2600
3DO|3DO Interactive Multiplayer
3DS|Nintendo 3DS
DC|Sega Dreamcast
DS|Nintendo DS
GB|Game Boy
GBA|Game boy Advance
GC|Nintendo Gamecube
GEN|Sega Genesis
GG|Game Gear
N64|Nintendo 64
NES|Nintendo Entertainment System
NG|Neo Geo
PC|Personal Computer
PCFX|PC-FX
PS|PlayStation
PS2|PlayStation 2
PS3|PlayStation 3
PS4|PlayStation 4
PSP|PlayStation Portable
PSV|PlayStation Vita
SAT|Sega Saturn
SCD|Sega CD
SNES|Super Nintendo Entertainment System
TG16|TurboGrafx-16
WS|WonderSwan
Wii|Nintendo Wii
WiiU|Wii U
X360|Xbox 360
XB|Xbox
XONE|Xbox One

## Rating

The Entertainment Software Rating Board (<b>ESRB</b>) was established in 1994 and is a system used in the United States and Canada to provide age and content ratings for video games. It is intended to assist consumers, particulary parents, in understanding the appropriateness of these games for different age groups. Below is a description of all the ratings in the dataset:
- <b>K-A:</b> was used until 1998 where it was then changed to <b>E</b>
  - <b>K-A:</b> will be modified to <b> E </b> for this analysis.

ESRB Rating|Description
-|:---
E|Everyone
M|Mature
T|Teen
E10+|Everyone Ages 10+
K-A|Kids to Adult
AO|Adults Only 18+
EC|Early Childhood (Ages 3+)
RP|Rating Pending

![](https://raw.githubusercontent.com/heiditm/heiditm.github.io/master/images/ESRB%20Rating%20Symbols.png)

![image](https://github.com/heiditm/heiditm.github.io/assets/56846204/6cedaa34-c08a-4a5e-89ba-685f8b7daa8b)
![image](https://github.com/heiditm/heiditm.github.io/assets/56846204/b58e497e-8069-45ee-910b-8aaa1ab69a51)
![image](https://github.com/heiditm/heiditm.github.io/assets/56846204/3264d421-8695-4fb6-b871-5458bf0d4db0)

![image](https://github.com/heiditm/heiditm.github.io/assets/56846204/fcc1ec3e-2663-48b3-aa82-31dffec909bd)

## Platform Insights
Category|Total Percentage in Top 10|Platforms Included
-|:-:|:-
Console|48.43%|PS2, PS3, Wii, X360, PS, XB, PC
Handheld| 25.02%|DS, PSP, GBA

## Publisher Insights
Country of Orgin/Region|Total Percentage in Top 10|Publishers Included
-|:-:|:-
American|20.83%|Electronic Arts (EA), Activision, THQ, Take-Two Interactive
Japan|22.82%|Namco Bandi Games, Konami Digital Entertainment, Nintendo, Sony Computer Entertainment, Sega
French|5.60%|Ubisoft

## Developer Insights
Skewed results as there are many companies under <b>Electronic Arts</b> which is included in the Top 10
Country of Orgin/Region|Total Percentage in Top 10|Developers Included
-|:-:|:-
American|21.73%|Electronic Arts (Inclusive of all EA), Visual Concept
Japan|3.77%|Konami Digital Entertainment, Capcom, Omega Force
French|3.02%|Ubisoft (Inclusive of all Ubisoft)

![image](https://github.com/heiditm/heiditm.github.io/assets/56846204/d17ead69-3f71-4075-8237-784e1881a061)
- Nintendo is a very strong competitor within a 40 year range having 22 years of highest global sales!
- Consoles has also kept their stance in being historically strong having 32 years of highest global sales!
![image](https://github.com/heiditm/heiditm.github.io/assets/56846204/f183700c-904b-4fcb-a150-ab30f24f035c)
- Ranked in the Top 5 global sales of the year:
  - All 5 games are by Nintendo
  - 4 of 5 games are console games
  - Pokemon is the only handheld game

![image](https://github.com/heiditm/heiditm.github.io/assets/56846204/5f26bc11-d40a-4c0a-a841-41e625e383a5)

Logistic Regression and Support Vector Machine models show to have very similar accuracy scores, but since Logistic Regression has a higher accuracy it is the better model to use for classification for platform type!
![image](https://github.com/heiditm/heiditm.github.io/assets/56846204/aed3a3bb-a6d1-4f9a-81bd-e91754432006)


![image](https://github.com/heiditm/heiditm.github.io/assets/56846204/da5b729b-41e9-4b03-a435-e9337312cff6)
