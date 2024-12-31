Tableau Visualization Setup Guide
1. Workspace Setup

Connect to Data:
Open Tableau -> Connect -> To a File -> Text File -> Load vgsales.csv.
Preview Data:
Rename columns if needed. Click "Sheet 1" to start.
2. Tableau Key Terms

Dimensions: Qualitative fields (e.g., Platform, Genre, Publisher).
Measures: Quantitative fields (e.g., Global_Sales, NA_Sales, Year).
Rows/Columns Shelves: Drag dimensions/measures here for visualization.
Marks: Customize shapes, sizes, colors, and labels.
Filters/Pages: Limit displayed data or segment views.
3. Basic Visualizations

Bar Chart (Global Sales by Genre):
Drag Genre to Columns, Global_Sales to Rows -> Right-click Global_Sales -> Measure -> Sum.
Sorting:
Sort by descending Global_Sales axis.
Filtering:
Drag Year to Filters -> Choose range (e.g., 2000-2016). Add Year to Pages for dynamic changes.
4. Dashboards and Advanced Visualizations

Line Chart (Sales Trend):
Drag Year to Columns, Global_Sales to Rows -> Add Genre to Marks -> Apply color.
Dashboard Creation:
Go to Dashboard tab -> Add multiple sheets -> Set size to "Automatic" -> Arrange visualizations (e.g., line chart for yearly sales, bar chart for top genres).

---


Tableau Guide for Excel File Connection and Joins
1. Connecting to Excel Files in Tableau:

Open Tableau -> Click Connect in the left pane.
Under To a File, choose Microsoft Excel.
Browse to and open Tableau Joins File.xlsx.
Tableau displays the sheets in the Data Source tab. Drag the relevant sheets to the workspace.
2. Dataset Overview (Tableau Joins File.xlsx):

Demographics Sheet: Contains EmployeeID, NameofEmployee, EmployeeAge, and EmployeeGender.
Salary Sheet: Contains EmployeeID and EmployeeSalary.
3. Types of Joins in Tableau:

Inner Join:

Purpose: Shows records with matching EmployeeID in both tables.
Steps: Drag Demographics and Salary sheets into the canvas. Ensure EmployeeID is selected for the join key. Choose Inner Join.
Result: Employees present in both tables.
Left Join:

Purpose: Returns all records from Demographics and matches from Salary. Missing matches have NULL in Salary.
Steps: Set the join type to Left Join.
Result: All employees appear, even if they lack salary data.
Right Join:

Purpose: Returns all records from Salary and matches from Demographics. Missing matches have NULL in Demographics.
Steps: Set the join type to Right Join.
Result: All salaries appear, even if employees are missing.
Full Outer Join:

Purpose: Includes all records from both tables. Missing matches result in NULL values.
Steps: Set the join type to Full Outer Join.
Result: Shows all employees and salaries, even without a match.
4. Visualizations After Joins:

Bar Chart (Number of Employees and Salaries):
Go to Sheet 1.
Drag NameofEmployee to Columns.
Drag EmployeeSalary to Rows.
Sort the chart in descending order.
Drag EmployeeSalary to Marks -> Add Color and Label.

---

Steps for Dashboard Design and Storytelling in Tableau
1. Creating a Dashboard in Tableau
Open Tableau and select the Dashboard tab at the bottom.
Drag your desired sheets (e.g., Sheet 1 and Sheet 2) into the workspace labeled Drop sheets here.
Adjust layout using containers:
Horizontal/Vertical Containers: Organize graphs, filters, and text.
Double-click titles to rename them meaningfully.
Add objects (e.g., text boxes, images) for context.
2. Adding Action Filters
Select a visualization (e.g., a line graph).
Click on the filter icon in the gray sidebar to make it interactive.
Test the filter by selecting data points and verifying changes in related visualizations.
3. Creating a Story in Tableau Public
Click New Story at the bottom right.
Drag sheets or dashboards into the "Drag a sheet here" pane.
Add captions to provide context, e.g., "Ontario had the highest health expenditure in Canada in 2016."
Highlight data points by selecting specific areas in a visualization, then click Update.
Use text boxes to emphasize insights.
4. Publishing a Tableau Public Workbook
Once satisfied with your workbook, go to File > Save to Tableau Public As.
Publish to Tableau Public for future use or sharing.
Small Story Example:
Introduction: Start with "Provincial Health Expenditure in 2016" to show the distribution.
Focus: Highlight Ontario’s spending using a map with annotations.
Trend Analysis: Use a line graph to show changes in Ontario’s expenditure from 1975–2018.
Conclusion: Show interactive insights, allowing users to explore provincial trends themselves.
This creates an engaging and insightful narrative tailored to your data!

---

[09:01, 31/12/2024] deva://127.4.7.8/: power bi

Power BI Overview: Components and Workflow

Components of Power BI:

Power BI Desktop: Tool for creating reports and visualizations on datasets.
Power BI Gateway: Keeps data fresh by connecting to on-premises data sources without moving the data.
Power BI Mobile Apps: Access and interact with data on Windows, iOS, and Android devices.
Power BI Service: Cloud-based platform for publishing reports and visualizations.
Workflow:

Designers collect and analyze data in Power BI Desktop and create reports.
Visuals are pinned to dashboards and shared via Power BI Service.
Business users access dashboards and reports for insights.
Key Elements:

Visualizations: Interactive charts to display data.
Semantic Models: Containers for data from sources like Excel, databases, or Salesforce.
Dashboards: Single-screen summaries of metrics using visuals from reports.
Reports: Multi-page visuals based on a semantic model.
Apps: Bundles of dashboards, reports, and models for sharing.
Power BI Desktop Interface:

Ribbon: Controls and options for report building.
Views: Report, Data, and Model views.
Canvas: Main area for creating visualizations.
Page Selector: Navigation for report pages.
Filters Pane: Apply data filters.
Visualizations Pane: Customize visuals and drill-through options.
Fields Pane: Displays available fields to add to the report.
Key Components of Power BI Desktop:

Power Query Editor: Cleans and transforms data from multiple sources.
Power View: Creates visually engaging charts and maps.
Power Map: 3D map visualizations for geospatial data.
Power Pivot: Data modeling and relationship creation using DAX.
Power Q&A: Natural language querying for in-depth data insights.


---

Creating Reports & Visualizations in Power BI

Common Charts in Power BI:
Bar Chart
Line Chart
Scatterplot
Sparkline
Pie Chart
Gauge
Waterfall Chart
Funnel Chart
Heat Map/Matrix
Histogram
Box Plot
Maps
Tables
Indicators
Area Chart
Radar/Spider Chart
Tree Map
Steps to Create Reports and Visualizations:
Open Power BI Desktop.

Load Data:

Click Get Data → Select Excel Worksheet (e.g., HR Data.csv).
Click Transform Data to open Power Query Editor.
Data Transformation:

Use the first row as headers.
Add a new column (e.g., attrition count) using Add Column.
Change the data type to Whole Number.
Click Close & Apply to load the transformed data into Power BI Desktop.
Build Reports:

KPI Chart:
Format visual: Add title, align, customize font colors, and borders.
Use Format Painter to apply similar formatting across visuals.
Pie Chart: Create using a similar process and apply the same formatting steps.
Additional Visuals:

Stacked Column Chart: Create a sort column if necessary.
Matrix: Format row/column headers and grand totals.
Doughnut Chart: Similar to Pie Chart, but with a blank center.
Slicers: Use to filter visuals on the page dynamically.
Key Features of Slicers:
Easy filtering with category, range, or date.
Display frequently used filters for quick access.
Highlight current filter state.
Allow focused reports by pairing slicers with critical visuals.
