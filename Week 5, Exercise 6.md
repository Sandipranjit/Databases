# Assignment 1
select max(elevation_ft) from airport;
![1](https://github.com/user-attachments/assets/b18a2bba-890b-4545-bd80-63ed5eb95f77)

# Assignment 2
select continent, count(*) from country group by continent;
![2](https://github.com/user-attachments/assets/f252d0e0-bf7a-4951-a552-1992bc3b1236)

# Assignment 3
select screen_name, count(*) from game left join goal_reached on id = game_id group by screen_name;
![3](https://github.com/user-attachments/assets/91a1de29-eeec-4695-948b-d242667ac19b)

# Assignment 4
select screen_name from game where co2_consumed = (select min(co2_consumed) from game);
![4](https://github.com/user-attachments/assets/6565e858-2332-4f8f-8e88-b9c6765c64f7)

# Assignment 5
select country.name, count(airport.id) as "count(*)" from country left join airport on country.iso_country =
airport.iso_country group by country.name order by count(airport.id) desc limit 50;
![5](https://github.com/user-attachments/assets/a15e741c-cead-4c97-a54c-7f1b632d686b)

# Assignment 6
select country.name from country left join airport on country.iso_country = airport.iso_country 
group by country.name having count(airport.id) > 1000;
![6](https://github.com/user-attachments/assets/41e7dbcc-8ae4-4adb-8cfb-c6e1d77a5e9a)

# Assignment 7
select name from airport where elevaton_ft in (select max(elevation_ft) from airport);
![7](https://github.com/user-attachments/assets/1ebb8678-df28-4ff6-9016-990eefeb8652)

# Assignment 8
select country.name from country join airport on country.iso_country = airport.iso_country 
where elevation_ft in (select max(elevation_ft) from airport);
![8](https://github.com/user-attachments/assets/5f87040f-ac11-46e8-81de-3a0c0b735f62)

# Assignment 9
select count(goal_id) as "count(*)" from goal_reached join game on goal_reached.game_id = game.id
where screen_name = "Vesa";
![9](https://github.com/user-attachments/assets/3b9173d2-36b2-4dc3-b736-718ba8267ab5)

# Assignment 10
select name from airport where latitude_deg in(select min(latitude_deg) from airport);
![10](https://github.com/user-attachments/assets/bc8c93a5-67a1-4e3e-922d-3d550c631c8e)
