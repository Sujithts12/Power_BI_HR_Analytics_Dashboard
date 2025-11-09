# Power BI HR Analytics Dashboard
    
📂 Download .pbix and open  with Microsoft Power BI Desktop.
👉 [Download it_company.pbix](it_company%20(2).pbix)


## 🔍 Project Overview

This project presents an interactive HR Analytics Dashboard built using Power BI, aimed at visualizing key HR metrics using a dummy dataset. The dashboard enables analysis of:

- Gender-wise employee distribution

- Total employee headcount

- Average salary and experience

- Technical skillset distribution

- Educational qualifications and certifications

- Working mode breakdown (Remote, Hybrid, Onsite)

- Employee source (how they joined)

- Interactive time slicers for trend analysis

## 🧰 Tools Used

- Power BI Desktop

- MS Excel (for data preparation)

- DAX (Data Analysis Expressions) for calculated measures

- Power Query Editor for data cleaning

## 🗂️ Dataset (Dummy) from https://mockaroo.com/


The dataset contains the following fields:

- Employee_ID

- Gender

- Salary

- Experience

- Skills (multiple)

- Education

- Certification_Status

- Working_Mode

- Joining_Source

- Company

- Joining_Year

Note: This is a dummy dataset created for learning and demonstration purposes only.


## 🧱 Steps to Build the Dashboard
## 1. 📥 Data Collection / Preparation

- created and imported dummy HR dataset in Excel.

- Ensured fields are clean and consistent (e.g., no nulls in critical fields like Gender, Company, Education).

- Loading the dataset into Power BI.

## 2. 🧹 Data Cleaning in Power Query

- Checked for  duplicates values.

- Correct data types (e.g., Salary as number, Joining Date as Date)
## 3. 🖼️ Adding Company Logos and Images

To enhance the dashboard visually and allow users to filter data by company using images, a separate image table was created.

## 🧱 Steps Taken:

- Created a 2 new table named CompanyImage with fields Company and Company_Image and Companylogo with fields Company and Company_logo

- The table was  created manually and imported from a Excel file.

- Established a relationship between:

    - Main Employee Table[Company] → Company_Image[Company]
    - Main Employee Table[Company] → Company_logo[Company]
- Used the Image URL field in visuals:

  - Set the column Data Category to Image URL (in column tools)

- Used Table visual to display images.

- Used image slicers  to allow dynamic filtering based on the selected company logo

- 🔍 Example Use Case:

    - When a user clicks on a company logo, the dashboard filters all visuals to show only data related to that selected company.

    - The company office image is dynamically shown in a separate card or image visual.

## 3. 📊 DAX

- Gender Count = COUNT(Employee[Gender])
- Headcount = COUNT(Employee[Employee_ID])
- AvgSalary = AVERAGE(Employee[Salary])
- AvgExperience = AVERAGE(Employee[Experience])
## 4. 📈 Report & Visualizations

- created the following visuals:

| Visual Element                    | Type              | Details                             |
| --------------------------------- | ----------------- | ----------------------------------- |
| **Total Headcount, Male, Female** | Cards             | With simple count and filters       |
| **Avg Salary & Experience**       | Cards             | Measures                            |
| **Technical Skills**              | Bar Chart         | Skills vs Count of Employees        |
| **Working Mode**                  | Stacked Bar Chart | Categories: Remote, Onsite, Hybrid  |
| **Education Pie Chart**           | Pie/Donut Chart   | B.Tech, M.Tech, MCA, MBA            |
| **Certifications**                | Guage              | Count of certified employees        |
| **Joining Source**                | Donut Chart       | Off Campus, Referral, College, etc. |
| **Year Filter**                   | Slicer            | To select by Joining Year           |
| **Company Image**                 | Image             | Inserted for aesthetics             |
| **Company Filter**                | Slicer (Buttons)  | Allows filtering per company logo   |

## 📌 Key Metrics Displayed

- Total Employees, Male Employees, Female Employees, Average Salary, Average Experience

- Skills Breakdown: Java, Python, Rust, SQL, etc.

- Education: Distribution of degrees

- Working Mode: Remote, Onsite, Hybrid

- Employee Source: Referral, Direct, Off-campus, College, Third-party

- Certifications: Certified and Non-certified



# Report Snapshot (Power BI DESKTOP) 
1.
![Bike Sales Dashboard 1](https://raw.githubusercontent.com/Sujithts12/Power_BI_HR_Analytics_Dashboard/main/image.png)
2.
![Bike Sales Dashboard 2](https://raw.githubusercontent.com/Sujithts12/Power_BI_HR_Analytics_Dashboard/main/image1.png)
3.
![Bike Sales Dashboard 3](https://raw.githubusercontent.com/Sujithts12/Power_BI_HR_Analytics_Dashboard/main/image2.png)
4.
![Bike Sales Dashboard 4](https://raw.githubusercontent.com/Sujithts12/Power_BI_HR_Analytics_Dashboard/main/image3.png)
5.
![Bike Sales Dashboard 5](https://raw.githubusercontent.com/Sujithts12/Power_BI_HR_Analytics_Dashboard/main/image4.png)
6.
![Bike Sales Dashboard 6](https://raw.githubusercontent.com/Sujithts12/Power_BI_HR_Analytics_Dashboard/main/image5.png)
7.
![Bike Sales Dashboard 6](https://raw.githubusercontent.com/Sujithts12/Power_BI_HR_Analytics_Dashboard/main/image6.png)
8.
![Bike Sales Dashboard 6](https://raw.githubusercontent.com/Sujithts12/Power_BI_HR_Analytics_Dashboard/main/image7.png)


## 👨‍💻 Author
Dashboard Created By: Sujith TS 

Date: 1st August 2025

## 📂 Download .pbix 

The report is provided in .pbix format and is designed to be opened using Microsoft Power BI Desktop.
Please ensure you have Power BI Desktop installed to view and interact with the dashboard.

👉 [Download it_company.pbix](it_company%20(2).pbix)

## 🎥 [Watch the interactive video demo on LinkedIn] 
- Link : https://l1nk.dev/u25pi

## 📌 Data Source 

The dataset used in this project was generated using Mockaroo
a tool for creating realistic looking mock data for development and testing purposes. The data is entirely synthetic and does not represent any real individuals or entities. https://mockaroo.com/
