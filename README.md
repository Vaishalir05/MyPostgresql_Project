# MyPostgresql_Project
---Json row 
select row_to_json(aa) from (select "ID", "Last_Name", "First_Name" from "TestDataBase"."SampleTB") as aa;

select row_to_json(row("ID", "Last_Name", "First_Name")) from "TestDataBase"."SampleTB";


---Recursive 
with recursive sam_Recursive as
(select * from "TestDataBase".med_memmbers where "ID" = 112)
select * from sam_Recursive;