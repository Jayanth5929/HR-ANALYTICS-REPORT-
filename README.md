
## problem statement 

The HR Analytics Dashboard is designed to provide comprehensive insights into the workforce of a company. The primary objective is to help HR professionals and business analysts understand key metrics related to employee demographics, attrition rates, job satisfaction, and overall workforce distribution. By leveraging these insights, organizations can identify trends, address potential issues, and make data-driven decisions to improve employee retention and satisfaction.


### Steps Followed
Data Loading and Preparation:
   - The dataset was loaded into Power BI Desktop and cleaned for accuracy.

2. Column Quality Tool:
   - Used the Column Quality tool under the Tools tab to assess the quality of the data.

3. Remove Unnecessary Columns:
   - Removed unnecessary columns, such as `YearsWithCurManager`, to streamline the dataset.

4. Group By Function:
   - Applied the Group By function to remove duplicate entries, ensuring the dataset's integrity.

5. Find and Replace:
   - Used the Find and Replace tool to rectify spelling mistakes in the dataset, such as correcting `travelRarely` to `TravelRarely` and `Taravel_rarely` to `TravelRarely`.

6. Add Additional Column for Attrition Count:
   - Added a new column `ATTRITION COUNT` using an IF condition to identify attrition cases.
     ```DAX
     ATTRITION COUNT = IF(HR_Analytics[Attrition] = "Yes", 1, 0)
     ```

7. Data Exploration and Profiling:
   - Column distribution, quality, and profiling were examined to understand data characteristics.

8. Visualization Design:
   - Various visuals such as bar charts, donut charts, and matrices were created to represent the data effectively.

9. Calculations and Measures:
   - Calculated columns and measures were developed using DAX expressions to derive meaningful insights from the raw data.

10. Dashboard Customization:
    - Filters and slicers were added for interactive analysis, allowing users to drill down into specific aspects of the data.

11. Publishing and Sharing:
    - The dashboard was published to Power BI Service for accessibility and collaboration.
