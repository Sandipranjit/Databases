# Assignment 1
update game
set co2_consumed = co2_consumed + 500,
    location = (select ident from airport where municipality = "Nottingham" and ident = "EGBN")
where screen_name = "Vesa" and location = "EGCC";
select * from game;
![1](https://github.com/user-attachments/assets/9ad491b6-226d-4ad4-b1ce-e63d97a82131)
