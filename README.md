# NBA GM Data

This is a dataset about current 30 NBA Executives as of the season 2019-2020. See my [full writeup](https://yifeihu.me/nba-gm-graph) that analyzed this data.

I manually collected and created the NBA GM dataset for this story. I relied heavily on Basketball Reference, RealGM, Pro Sports Transactions Archive, and media guides published by teams.

## Data Dictionary

### gm.csv

This table contains facts about the GMs, where each row is a GM.

Name|Type|Description
---|---|---
Team|String|Team name
Name|String|GM's name
Current Start Date|Date|Start date of GM's current position
Current Tenure|Number|Number of years of GM's current tenure, derived from Current Start Date (This needs to be updated!)
Championships as GM|Number|Number of NBA championships won as GM
Executive of the Year|Number|Number of times GM has won Executive of the Year Award
Ex NBA Player|Boolean|Whether GM played in the NBA
Ex College Player|Boolean|Whether GM played college basketball
Ex NBA Coach|Boolean|Whether GM coached in the NBA
Ex College Coach|Boolean|Whether GM coached in college basketball
Ex Agent|Boolean|Whether GM was a player agent
Ex Scout|Boolean|Whether GM was a scout for an NBA team
Ex Video|Boolean|Whether GM edited videos for an NBA team
MBA|Boolean|Whether GM holds an MBA degree
JD|Boolean|Whether GM holds a JD degree
Promoted|Boolean|Whether GM was internally promoted to current position
Sloan|Boolean|Whether GM attended the Sloan Sports Analytics Conference in the past

### gm_to_team.csv

This table contains the past experiences of the GMs in the NBA, where each row records where a GM worked in the past from year X to year Y.

Name|Type|Description
---|---|---
GM|String|GM's name
Team|String|Team name
Note|String|Notes about the record
From|Number|Start year of the experience
To|Number|End year of the experience
Reference|String|Link to the source where the info was obtained
