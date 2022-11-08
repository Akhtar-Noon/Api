create table weather
(
  id int,
  recordDate date,
  temperature int,
  primary key (id)
  );

 create table weather_details
 (
   Desc_id int,
   tempID int,
   Description varchar,
   primary key (Desc_id),
   foreign key (tempID) References Weather 
   );
   
   
  Alter table Weather_details
rename tempID to TemperatureID;
   
  insert into weather 
Values
(4,'13-3-2022',30),
(5,'19-2-2022',45),
(6,'18-3-2022',20),
(7,'18-2-2022',55),
(9,'16-3-2022',20),
(8,'17-2-2022',65)
;
