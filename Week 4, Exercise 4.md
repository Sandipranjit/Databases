# Assignment 1
select country.name as "country name", airport.name as "airport name" from country inner join airport on 
country.iso_country = airport.iso_country where airport.iso_country = "FI" and scheduled_service = "yes";
![1](https://github.com/user-attachments/assets/0cd49c3a-447a-4a4f-8b18-36f9998c8050)

# Assignment 2
select screen_name, name from airport inner join game on airport.ident = game.location;
![2](https://github.com/user-attachments/assets/a4e3d214-56e8-40ce-b84d-c131f49d7ff6)

# Assingment 3
select screen_name, coountry.name as "name" from game inner join airport on airport.ident = game.location 
inner join country on country.iso_country = airport.iso_country;
![3](https://github.com/user-attachments/assets/b559965a-69b5-44ad-8f74-20a0b9f3e3ac)

# Assignment 4
select name, screen_name from airport left join game on airport.ident = game.location where airport.name like "%Hels%";
![4](https://github.com/user-attachments/assets/b9df4236-9d5f-4b8a-a5b5-0f70f3b41431)

# Assignment 5
select name, screen_name from goal left join goal_reached on goal.id = goal_reached.goal_id 
left join game on game.id = goal_reached.game_id;
![5](https://github.com/user-attachments/assets/8dc44c69-b556-4e2e-953c-ffd233fe2e2b)
