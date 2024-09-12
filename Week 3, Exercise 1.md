# Assignment 2
select name, type from airport where iso_country = "FI";
![Tehtävä 2](https://github.com/user-attachments/assets/34f21e62-7e76-4132-b724-6794291dd429)

# Assignment 3
select name from airport where iso_country = "FI" order by name;
![Tehtävä 3](https://github.com/user-attachments/assets/10545b7a-746f-495a-9974-33e1055791ee)

# Assignment 4
select name, type from airport where iso_country = "FI" order by type, name;
![Tehtävä 4](https://github.com/user-attachments/assets/75aeca79-2149-4c8b-b83e-32b1ca974a1c)

#Assignment 5
select name from country where name like "F%";
![Tehtävä 5](https://github.com/user-attachments/assets/5cfff267-3766-40a5-9b92-087aee98422d)

#Assignment 6
select name from country where name like "%F%";
![Tehtävä 6](https://github.com/user-attachments/assets/61faac9c-31fe-4be1-91da-480de1f53c03)

#Assignment 7
select location from game where screen_name = "Vesa";
![Tehtävä 7](https://github.com/user-attachments/assets/db23a64e-35f4-4c01-b5dc-e90ff3acb973)

# Assignment 10
select screen_name, co2_budget, co2_consumed, @co2_left :=(co2_budget - co2_consumed) as co2_left from game where screen_name = "Ilkka";
![Tehtävä 10](https://github.com/user-attachments/assets/f43c6250-5535-47c3-a809-2f5fe04a0fe5)
