# Assignment 1
select country.name as "country name", airport.name as "airport name"  from country, airport where country.iso_country = airport.iso_country  and country.name = "Iceland";
![1](https://github.com/user-attachments/assets/473e263d-425a-4fcb-adba-425a188da7f3)

# Assignment 2
select airport.name as "airport name"  from airport, country  where airport.iso_country = country.iso_country  and airport.type = "large_airport"  and country.name = "France";
![2](https://github.com/user-attachments/assets/48e523c6-64dc-4843-a76f-eddd19acb4ac)

# Assignment 3
select country.name as "country_name", airport.name as "airport_name" from country, airport where country.iso_country = airport.iso_country and country.continent = "AN";
![3](https://github.com/user-attachments/assets/3850c8a1-6bd3-46d8-b4ac-53f1d9709852)

# Assignment 4
select airport.elevation_ft from airport, game where airport.ident = game.location and game.screen_name = "Heini";
![4](https://github.com/user-attachments/assets/706e49e7-269f-486e-ba60-dd0cfa928219)

# Assignment 5
select airport.elevation_ft*0.3048 as "elevation_m" from airport, game where airport.ident = game.location and game.screen_name = "Heini";
![5](https://github.com/user-attachments/assets/05afc33f-5907-41d4-b477-a95bfc21de42)

# Assignment 6
select airport.name as "name" from airport, game where airport.ident = game.location and game.screen_name = "Ilkka";
![6](https://github.com/user-attachments/assets/42f18cd6-006f-45ae-a879-96873f4f56cc)

# Assignment 7
select country.name as "name" from country, game, airport where country.iso_country = airport.iso_country and airport.ident = game.location and game.screen_name = "Ilkka";
![7](https://github.com/user-attachments/assets/e8c5b2d0-6266-4f00-9f51-e4dae46501d3)

# Assignment 8
select goal.name as "name" from goal, game, goal_reached where goal.id = goal_reached.goal_id and goal_reached.game_id = game.id and game.screen_name = "Heini";
![8](https://github.com/user-attachments/assets/ce7a950e-e5ce-44f3-8c0d-ca135a63e763)

# Assignment 9
select airport.name as "name" from airport, game, goal, goal_reached where airport.ident = game.location and game.id = goal_reached.game_id and goal.id = goal_reached.goal_id and game.screen_name = "Ilkka" and goal.name = "clouds";
![9](https://github.com/user-attachments/assets/78ddd9a4-f59b-49c3-ab61-3d1387c59643)

# Assignment 10
select country.name as "name" from airport, country, game, goal, goal_reached where airport.ident = game.location and game.id = goal_reached.game_id and goal.id = goal_reached.goal_id
and airport.iso_country = country.iso_country and game.screen_name = "Ilkka" and goal.name = "clouds";
![10](https://github.com/user-attachments/assets/9005fc14-0372-47d5-9a07-aaa6e78aaf2c)
