# Assignment 1
select * from goal;
![Tehtävä 1](https://github.com/user-attachments/assets/edb2c04a-be84-4f7f-850f-f129f066be2c)

# Assignment 2
select name, type from airport where iso_country = "FI";
![Tehtävä 2](https://github.com/user-attachments/assets/182a7811-533c-4a51-8bec-dad200a2ff04)

# Assignment 3
select name from airport where iso_country = "FI" order by name;
![Tehtävä 3](https://github.com/user-attachments/assets/6953385a-d6e0-4bab-83db-efd41980086f)

#Assignment 4
select name, type from airport where iso_country = "FI" order by type name;
![Tehtävä 4](https://github.com/user-attachments/assets/55a3c652-bd26-406b-bf42-825a333e7826)

# Assignment 5
select name from country where name like "F&";
![Tehtävä 5](https://github.com/user-attachments/assets/6b1d02cd-1f21-4dc2-884a-c4ea12c39551)

# Assignment 6
select name from country where name like "%F%";
![Tehtävä 6](https://github.com/user-attachments/assets/885bff5a-fb30-4597-9830-34bf4ec3cd1d)

# Assignment 7
select location from game where screen_name = "Vesa";
![Tehtävä 7](https://github.com/user-attachments/assets/c0f9f10e-b52b-4e09-aa3e-6d8fa534c9b1)

# Assignment 8
select co2_consumed from game where screen_name = "Ilkka";
![Tehtävä 8](https://github.com/user-attachments/assets/6d55bcb8-e3e0-4b6d-ab82-fdc8ca49443b)

# Assignment 9
select co2_budget from game limit 1;
![Tehtävä 9](https://github.com/user-attachments/assets/6888989f-379e-4ee8-bd6d-838452f4d2df)

# Assignment 10
select screen_name, co2_budget, co2_consumed, @co2_left :=(co2_budget - co2_consumed) as co2_left from game where screen_name = "Ilkka";
![Tehtävä 10](https://github.com/user-attachments/assets/8e61d27a-f310-424c-9990-b478b43ab177)





