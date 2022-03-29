# MyPostgresql_Project
---Json row 
select row_to_json(aa) from (select "ID", "Last_Name", "First_Name" from "TestDataBase"."SampleTB") as aa;

select row_to_json(row("ID", "Last_Name", "First_Name")) from "TestDataBase"."SampleTB";

