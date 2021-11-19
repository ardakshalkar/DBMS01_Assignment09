# Assignment 09
## P01
**P01.A** Display standings table like in table below:
|Title|played|won|draw|lost|goals|points|
|-----|------|---|----|----|-----|------|
|Real Madrid|3|2|1|0|9-4|7|
|Liverpool|3|1|1|1|3-5|4|
|Man Utd|3|0|3|0|2-2|3|
|Barcelona|3|0|1|2|2-5|1|
---
**P01.B** Display Match calendar like in table below:
|id|Teams|score|round|
|--|-----|-----|-----|
|1|Barcelona : Real Madrid|1 : 3|1|
|2|Liverpool : Man Utd|0 : 0|1|
|3|Real Madrid : Man Utd|2 : 2|2|
|4|Liverpool : Barcelona|2 : 1|2|
|5|Liverpool : Real Madrid|1 : 4|3|
|6|Man Utd : Barcelona|0 : 0|3|


---
## P02
* **P02.A** When new user is inserted, it should create new account, with money -500$.
* **P02.B** When new company is inserted, it should create new account with money `-10000$`, if it is from Kazakhstan, and `-20000$` for other countries.
* **P02.C** When user, or company deleted the corresponding account is now will be belong to DeletedCompany, with `CompanyID = 11`
* **P02.D** When account's user value is changed it should be stored to Logs_Account_Change
* **P02.E** Do not let delete 
---
## P03
* **P03.A** When new `Club` is inserted,  new row to `Standings` should be inserted with club_id same to clubs id.
* **P03.B** Create triggers that when you insert new data to `Matches`, it should update standings, so the team which won should got +3 points to score (or +1 if draw), and scored_goals, conceded_goals, won, draw, lost fields are also should be update respectively.
* **P03.C** Also create trigger that update, delete on `Matches` table which should update `Standings` table respectively.
* **P03.D** Create triggers for insert, update, delete for `Club` table. 
    * When new club inserted should insert corresponding row to `Standings` table.
    * When delete club it should also delete corresponding `Match` fields.