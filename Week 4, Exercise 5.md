# Assignment 1
select country.name from country where country.iso_country in (select airport.iso_country from airport 
where airport.name like "Satsuma%");
![1](https://github.com/user-attachments/assets/7210503a-d440-4735-b515-6e1b7e34682f)

# Assignment 2
select name from airport where airport.iso_country in (select country.iso_country from country 
where name = "Monaco");
![2](https://github.com/user-attachments/assets/90b75c56-120a-4351-9ab0-486210bde73e)

# Assignment 3
select screen_name from game where game.id in (select game_id from goal_reached where goal_id in (
select id from goal where name = "Clouds"));
![3](https://github.com/user-attachments/assets/7fb8b990-0924-4e33-81c3-055199fb9fca)

# Assignment 4
select name from country where iso_country not in (select iso_country from airport);
![4](https://github.com/user-attachments/assets/74d93972-7cbb-454c-a044-5198daf3d167)

# Assignment 5
select name from goal where id not in (select goal_id from goal_reached where game_id in (
select id from game where screen_name = "Heini"));
![5](https://github.com/user-attachments/assets/fc65091d-474c-4756-bf7a-fab19feb595a)
