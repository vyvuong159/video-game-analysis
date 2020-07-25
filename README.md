## Introduction
- This project is an assignment of the Data Scientist training program by Practicum - Yandex. 
- This project analyzes data on game sales in North America, Europe, Japan and other regions to see which game platform is more profitable, and how expert and user reviews affect the sale of these games.
- This project is the foundation for the marketing department to plan their advertising campaign for the next period. 

## Research questions
- How long does it generally take for new platforms to appear and old ones to fade?
- Which platforms are leading in sales? Which ones are growing or shrinking? 
- How do expert and user reviews affect the sales of game broken down by platform?
- Do Entertainment Software Rating Board (ESRB) ratings affect sales in each of the following regions: North America, Europe and Japan. The ESRB assigns age and content ratings to consumer video games.
- Are average user ratings of the Xbox One and PC platforms the same?
- Are average user ratings for the Action and Sports genres the same?

## Tasks 
- Identify and imputing for missing values
- Replace data type
- Identify and dropping duplicates
- Conduct exploratory data analysis: create graphs (lineplot, scatterplot, histogram) and calculate correlation coefficients
- Test the hypotheses

## Data description
- Source: Yandex provides the data which is extracted from [Kaggle](https://www.kaggle.com/gregorut/videogamesales).
- The dataset contain info of: User and expert reviews, genres, platforms (e.g. Xbox or PlayStation), ESRB rating categories and historical data on game sales are available from open sources.
- Metadata

| Column name                                  | Description                                                  | Data type |
|----------------------------------------------|--------------------------------------------------------------|-----------|
| Name                                         | The games name                                               | String    |
| Year_of_Release - Year of the game's release | Platform of the games release (i.e. PC,PS4, etc.)            | Float     |
| Genre -                                      | Genre of the game                                            | String    |
| NA_Sales -                                   | Sales in North America (in millions)                         | Float     |
| EU_Sales -                                   | Sales in Europe (in millions)                                | Float     |
| JP_Sales -                                   | Sales in Japan (in millions)                                 | Float     |
| Other_Sales -                                | Sales in the rest of the world (in millions)                 | Float     |
| Critic_Score                                 | Review score of experts (maximum of 100)                     | Float     |
| User_Score                                   | Review score of users (maximum of 100)                       | Float     |
| Rating                                       | ESRB Rating (eg. Everyone, Everyone 10+, Teen, Mature, etc.) | String    |

## Conclusions
- It generally takes around 4-6 years for a new platforms to reach its peak in sale, and it takes around 5-7 years for an old platform to fade, i.e. reach its lowest in sale (approximately zero sales).
- In the period from 2005-2016, X360, PS3 and Wii are the top 3 platforms leading in sales. The following platforms are shrinking: PS2, Wii, DS, X360, PS3, PSP. The other platforms that ended their life earlier (before 2008) are: XB, GBA, GC, and DC. Though there is a tendency for decreasing, the following platforms have not reached their peak (because it usually takes 4-6 years to reach the peak), so there is a chance for these platforms to rise after 2016, or at least last for several more years: PS4, XOne, 3DS, PSV, WiiU.
- There are relatively weak positive correlations between user and professional reviews with total sales. Professional reviews seem to have stronger effect on total sale than user reviews.
- The relationship between ESRB rating and video game sales 
  - North America: ESRB ratings affect sales in North America. It seems that 'everyone' category are the most favorite one, and therefore the most profitable in all 3 regions. 'Mature' category ranks second.
  - Europe: ESRB ratings affect sales in Europe. 'Everyone' category ranks first, followed by 'Mature'.
  - Japan: ESRB ratings affect sales in Japan. 'Everyone' also ranks first, followed by 'Teen'.
- XBox One and PC platforms enjoy the same level of user review while Action and Sports genres differ in user reviews where Action games tend to have higher review from users.
