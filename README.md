# My-Teableau-learning

Step 1: Understand What Tableau Is

Tableau is a data visualization and business intelligence tool.
It helps convert raw data into easy-to-understand interactive dashboards.

Key products:

Tableau Desktop → Create visualizations
Tableau Public → Free version (for practice)
Tableau Server / Tableau Online → Share dashboards

Step 2: Learn the Tableau Interface

🧭 Main components:

Data Pane – shows your fields (dimensions & measures)
Shelves – Columns, Rows, Filters, Pages, Marks, etc.
Marks Card – customize color, size, label, detail, tooltip
Show Me Panel – suggests chart types
Worksheet / Dashboard / Story tabs – where you create visualizations


Step 3: Connect and Prepare Data

Import data from Excel, CSV, Google Sheets, SQL, etc.
Tableau auto-detects data types (Number, String, Date…)
Data types icons:

# → Number
Abc → Text
📅 → Date
Clean data using:
Rename columns
Change data types
Create calculated fields
Remove nulls

Step 4: Understand Dimensions and Measures

Dimensions – Categorical fields (e.g. Region, Category)
Measures – Numeric fields (e.g. Sales, Profit)
Tableau automatically aggregates measures (SUM, AVG, etc.)

Step 5: Basic Charts

✅ Learn to create these visualizations:

Chart Type	When to Use	How to Create
Bar Chart	Compare categories	Drag Category → Columns, Sales → Rows
Line Chart	Show trends over time	Date → Columns, Sales → Rows
Pie Chart	Show part-to-whole	Category → Color, Sales → Angle
Map	Geographical data	State/City → Detail, Sales → Color
Scatter Plot	Relationship between 2 measures	Profit → Columns, Sales → Rows

Step 6: Filters and Sorting

Filters: Exclude/include data
Drag a field to Filters shelf
Quick Filters: Right-click field → Show Filter
Sorting: Click on sort icon in the axis or header

Step 7: Calculated Fields

Use formulas to create new fields:
Profit Ratio = SUM([Profit]) / SUM([Sales])

IF [Sales] > 1000 THEN "High" ELSE "Low" END

Types of calculations:

Row-level
Aggregate
Table calculations (e.g. % of Total, Running Total)

Step 8: Combine Data

Joins: Combine multiple tables (inner, left, right, full)
Blends: Combine data from different sources
Unions: Stack similar data (same structure)

Step 9: Dashboards & Interactivity

Dashboard = multiple sheets on one screen

Add:

Filters
Parameters
Actions (Filter Action, Highlight Action, URL Action)
Keep it clean and interactive.

Step 10: Publish & Share

Save workbook as .twb or .twbx
Publish to Tableau Public or Tableau Server
Export as PDF or Image

Step 11: Practice Projects

Try small projects:
Superstore Sales Dashboard
COVID-19 Data Tracker
HR Employee Analysis
Finance KPI Dashboard





**----Steps to Create a Hierarchy in Tableau----**

A hierarchy is useful when you have fields that represent different levels of detail, for example:
Geography: Country → State → City
Time: Year → Quarter → Month → Day
Organization: Department → Team → Employee

Method 1 – Using Drag and Drop

In the Data pane, locate the related fields.
Drag one field (e.g., State) on top of another (e.g., Country).

Tableau will prompt:

👉 “Create Hierarchy”

Enter a name for your hierarchy (e.g., Geography).
Now both fields will appear nested under that hierarchy.

<img width="1366" height="728" alt="image" src="https://github.com/user-attachments/assets/143f8f22-934c-4cf8-824c-d9ce37707f43" />

Method 2 – Using the Right-Click Menu

Right-click on the field that should be the top level (e.g., Country).

Select Hierarchy → Create Hierarchy.

Give the hierarchy a name.

Drag other related fields (e.g., State, City) into the hierarchy.

<img width="1366" height="729" alt="image" src="https://github.com/user-attachments/assets/e5cafec8-0500-4280-bcbe-ebb59196a08f" />

**----Steps to Create a Group in Tableau----**

Method 1: Create a Group from the Data Pane

Open Tableau and connect to your dataset.

In the Data Pane (left sidebar), locate the dimension you want to group (for example, Category or Region).

Right-click the dimension → select Create → Group.

In the Create Group dialog box:

Select the members you want to group together.

Click Group to combine them.

Optionally rename the group (e.g., "North Regions").

Click OK.

A new field (e.g., Category (group)) appears in the Data Pane — you can now use it in your visualizations.

<img width="1366" height="730" alt="image" src="https://github.com/user-attachments/assets/cecea428-4a01-451f-b0f9-435043b90753" />


Method 2: Create a Group from a View (Visualization)

Drag your desired dimension to Rows or Columns and build a basic view (e.g., a bar chart).

In the view, Ctrl + Click (or Cmd + Click on Mac) to select multiple members you want to group.

Right-click one of the selected members → choose Group.

Tableau creates a new group automatically and adds it to the Data Pane.

You can edit or rename the group later.

<img width="1366" height="730" alt="image" src="https://github.com/user-attachments/assets/88c8d5d5-44cc-49e7-99c1-e7b04769cbd4" />


<img width="1366" height="731" alt="image" src="https://github.com/user-attachments/assets/4bd468e5-5966-42ad-99d3-09385d9f9ead" />


**What is a Parameter in Tableau?**

A Parameter is a dynamic input that allows users to replace a constant value in a calculation, filter, or reference line.
Example: You can use a parameter to let users select a number, a date, or a category that changes the visualization dynamically.

different ways to create Parameter

<img width="1366" height="730" alt="image" src="https://github.com/user-attachments/assets/8abd35b4-283c-4ae7-97b7-9c71969c50b1" />

<img width="1366" height="731" alt="image" src="https://github.com/user-attachments/assets/856eecfa-5ac0-4712-8073-c1f021c6bdca" />

<img width="1366" height="732" alt="image" src="https://github.com/user-attachments/assets/5b8f5f6b-8618-466a-a987-ec8fb83b1f63" />

<img width="1366" height="733" alt="image" src="https://github.com/user-attachments/assets/c855c306-899a-4f0c-bffd-3f0b612981af" />


**Example of parameter set bar chart**


