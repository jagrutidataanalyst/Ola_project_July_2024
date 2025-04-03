# Ola_project_July_2024 (Dashboard Project)


### Dashboard Link : https://app.powerbi.com/groups/me/reports/9973e481-23da-4c8f-b753-e30c8f341bfe/40a766c2a26e09b2be39?experience=power-bi

## Problem Statement

The transportation service provider aims to analyze ride patterns, customer behavior, and revenue trends to improve service quality, optimize operations, and enhance customer satisfaction. This study uses Power BI to extract insights from ride data to make data-driven decisions.

### Steps followed 

### Steps for Ola Project in Power BI

#### Step 1: Load Data into Power BI Desktop
- Load the dataset (CSV file) into Power BI Desktop.

#### Step 2: Open Power Query Editor
- Navigate to the **View** tab under **Data Preview** section.
- Enable **Column Distribution**, **Column Quality**, and **Column Profile**.
- Select **Column profiling based on the entire dataset** to analyze all rows.

#### Step 3: Data Cleaning
- Identify and handle missing values.
- Check for duplicate values and remove them if necessary.
- Format data types correctly (Date, Time, Currency, etc.).

### Step 4: Creating Calculated Columns  
- Use **DAX** to create new calculated columns for enhanced insights.  
- Derive additional fields such as ride duration, fare per km, or peak hour indicators.  
- Example: Calculate fare per km  
  ```DAX
  Fare_Per_KM = Ola_Rides[Fare] / Ola_Rides[Distance]

#### Step 5: Creating Measures
- Calculate total rides:
  ```DAX
  Total Rides = COUNT(Ola_Rides[Ride_ID])
  ```
- Calculate average ride fare:
  ```DAX
  Avg Fare = AVERAGE(Ola_Rides[Fare])
  ```
- Calculate total distance covered:
  ```DAX
  Total Distance = SUM(Ola_Rides[Distance])
  ```

#### Step 6: Adding Visuals
- Add **Card Visuals** for key metrics:
  - Total Rides
  - Average Fare
  - Total Distance
  
- Add **Bar Chart** for ride distribution by city.
- Add **Pie Chart** for ride distribution by customer type (New/Returning).
- Add **Line Chart** to show monthly ride trends.
- Use **Slicers** for filtering based on City, Ride Type, and Date.

#### Step 7: Formatting and Branding
- Apply a theme under **View** tab.
- Insert text boxes for project title and key insights.
- Add company logo using **Insert > Image**.

#### Step 8: Publishing the Report
- Publish the report to **Power BI Service**.
- Share the dashboard with stakeholders.

### Insights and Analysis
1. **Total Rides Analysis**
   - Identify peak ride hours and locations.
   (https://github.com/user-attachments/assets/0fe74803-d812-47a9-9104-b444f980b90c)
2. **Customer Preferences**
   - Analyze ride preferences based on customer type.
   (https://github.com/user-attachments/assets/19a7c691-24ab-41b1-b57a-92f8a3983448)
3. **Revenue Trends**
   - Track the revenue pattern over different time periods.
   (https://github.com/user-attachments/assets/d282796c-2464-4ce5-8c4c-c0a6c427f4bc)
4. **Cancellations and Ratings**
   - Compare ride frequency across cities.
   (https://github.com/user-attachments/assets/b92e303c-833f-48a5-a471-4a2faf1f44a3)
(https://github.com/user-attachments/assets/438a13d2-cb9b-4934-ac44-97d1815be3b9)


      
