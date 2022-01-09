
# HR Management Analysis 

## Project Description:
This project deals with 4 years of HR data(source data) which has been collected from a company's HR Database.The data contains each and every information related to the employees of that company.Now our aim in this project is to design a HR Management Dashboard in Excel which will provide a proper insight about the employees and the company's HR management status.All the data are present in the "HR_Source_Data" folder.

## Project Requirement:
- Build an interactive Dashboard using the source data folder which will visualize the following analysis-
    
            1.Yearly and quarterly new hires and the active employees.
            2.Full time and Part time active employees, classified based on the ethnic group and gender.
            3.How many yearly bad hires and terminated employees are there.
            4.Yearly voluntary and involuntary termination.
            5.Region wise Full time and Part time active employees.
            6.Average tenure months classified based on ethnic group and gender.
            7.In the dashboard headline section provide some informative statistics which will include-
              % of Male and Female employees in total employees,% of male and female according to pay type,Job type(Full time or part time),age group and turnover(yearly termination per active employee ).
- Add some necessary slicers to the Dashboard.
- The Dashboard should be dyanmic so that whenever new HR data is added to the source folder, the Dashboard gets updated automatically.

## Project Walkthrough:
### Insert the data from the source folder:

![insert data](https://user-images.githubusercontent.com/80168505/144270922-ee303a12-1bcc-481a-a2aa-a8f3ef628b15.png)

### Combine and transfrom the data:

![combine and tranform data](https://user-images.githubusercontent.com/80168505/144271297-8276b88e-b2d2-46b1-8be6-5b0ae24e6879.png)

### Made some necessary changes in the query editor:

![power query editor](https://user-images.githubusercontent.com/80168505/144271633-3020e9de-1342-4822-92fd-9bac99e95b57.png)

### Close the query and load the data, keeping the data connection only and adding the data to the data model:

![query save and close option](https://user-images.githubusercontent.com/80168505/144273651-22fa6936-60d0-434f-a8c9-4526e6b427a7.png)

### Create a chart of total active employees:
- Create a pivot table 
- Name the table - Actives
- Group the dates by year and quarter
    ![actives1](https://user-images.githubusercontent.com/80168505/144275798-b42244ea-85c0-481c-a82c-6a3f540191bc.png)
- Create 2 new measures
1. Active Employees
![actives2](https://user-images.githubusercontent.com/80168505/144276665-a8e0cce9-91c5-429e-bde9-7c07491b4125.png)

2. New Hires
![actives3](https://user-images.githubusercontent.com/80168505/144276686-19ca6f08-7dfe-4491-9eeb-c6ec750266f0.png)
- Insert bar chart
![actives4](https://user-images.githubusercontent.com/80168505/144283066-126dae22-d5ca-482e-a8ae-e7a66f7dce23.png)

### Create a chart of total active employees by ethnicity:
- Create a pivot table 
- Name the table - Ethnicity
- Filter the ethnic group based on gender and full time/part time
![ethnicity1](https://user-images.githubusercontent.com/80168505/144284236-93986c85-99b8-4853-88ce-d1b07025b755.png)
- Insert  bar chart
![etnicity2](https://user-images.githubusercontent.com/80168505/144284477-bf689b06-c561-4ac9-9dbe-5a639bf4e6dc.png)
### Create a chart of Separations and Bad Hires:
- Create a new measure and name it "Separation",which basically calculates  how many employees got terminated
![separations1](https://user-images.githubusercontent.com/80168505/144285715-48628ecb-59db-486a-b3e1-e3d9aaff14cf.png)
- Create a pivot table 
- Name the table - Separations
- Group the dates by year
![separations2](https://user-images.githubusercontent.com/80168505/144286666-c394e50f-4d94-486a-9a61-dc3f9f30d2f5.png)
- Insert a bar chart
![separations3](https://user-images.githubusercontent.com/80168505/144286908-97670f5c-72ba-4651-959a-b196c197ca88.png)
### Create a chart of Termination Reason:
- Create a pivot table
- Name the table - TermReason
- Group the dates by year
- Add TermReason in the column field
![termreason1](https://user-images.githubusercontent.com/80168505/144291947-dc6a5d07-75df-4dc7-8b23-9b0a41788966.png)
- Insert a bar chart
![termreason2](https://user-images.githubusercontent.com/80168505/144292126-3d003aa8-b490-43b6-8c6a-a0523f8127b2.png)
### Create a chart of region wise active employees:
- Create a pivot table 
- Name the table - Region
- Group the region wise active employees 
- Filter the table based on their job type- Full time(FT) / Part time (PT)
![region1](https://user-images.githubusercontent.com/80168505/144293033-6a0286a2-c75e-4292-9eb1-de96ae194432.png)
- Insert a horizontal bar chart
![region2](https://user-images.githubusercontent.com/80168505/144293437-59540375-a905-4d29-ad86-24f8f3a62805.png)
### Create a chart of average Tenure (in months):
- Create a new measure and name it "Avg. Tenure Months", which basically calculates avg. tenure of employees
![tenure1](https://user-images.githubusercontent.com/80168505/144294725-8dee23de-d405-4f09-889e-8489c26b07f4.png)
- Create a pivot table
- Name the table - Tenure
- Group the Male and Female employees based on their ethnicity
-  Filter the table based on their job type- Full time(FT) / Part time (PT)
![tenure2](https://user-images.githubusercontent.com/80168505/144295247-354ffd92-462f-4c3d-967e-9898a65f5848.png)
- Insert a bar chart
![tenure3](https://user-images.githubusercontent.com/80168505/144295484-191ec16d-7532-4152-b78e-3c1522f48a93.png)
### Create a Dashboard sheet and paste the above created charts:
- Create a separate sheet for building the final Dashboard
- Move all the charts to this Dashboard sheet
- In the dashboard headline section insert some informative statistics along with the visualization-
        
        1. % of Male and Female employees in total employees
        2. % of male and female according to pay type
        3. % of male and female according to Job type(Full time or part time)
        4. % of male and female according to age group
        5. % of male and female according to turnover 
    ![headlines](https://user-images.githubusercontent.com/80168505/144297101-6d797de6-242c-4463-9262-deddc9208b2f.png)

### Add Slicers:
- Add 5 slicers to the dashboard
  
      1.Full Time / Part Time
      2.Gender
      3.Region
      4.Ethnicity
      5.Year
    ![slicer1](https://user-images.githubusercontent.com/80168505/144298153-0d74b09b-975e-4ad9-a6cf-e7350830d077.png)
    ![slicer2](https://user-images.githubusercontent.com/80168505/144298167-f843f338-9294-4f61-87b0-0336a22de424.png)
- Link the slicers with the charts

## The Final Dashboard looks like --

![final dashboard](https://user-images.githubusercontent.com/80168505/144298816-9173a621-a871-4255-a7ee-e0d870110637.png)







