# Power-BI-Dashboards" >> README.md
  

### Dashboard Link :  

## Problem Statement

 Blinkit, a popular quick commerce platform, faces growing concerns over the lack of transparency and reliability in its product review system. Users have reported inconsistencies between product reviews and actual product quality, suggesting the presence of "fake" or misleading reviews. These inflated reviews may give customers false expectations, leading to dissatisfaction and diminished trust in the platform. Additionally, the absence of proper moderation for product feedback makes it easier for vendors to manipulate ratings, further compromising the credibility of the system. As customer trust is vital to the success of online platforms, the prevalence of unreliable reviews could lead to a decline in user retention and brand loyalty. Blinkit must address these issues by enhancing its review moderation policies, implementing verification mechanisms, and ensuring that customer feedback remains authentic and trustworthy to maintain its competitive edge in the market.

### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a xlsx file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : It was observed that in none of the columns errors & empty values were present except column named "Item Fat Content".
- Step 5 : For calculating some measures

Following DAX expression was written for the same,
        
        Total sales = SUM('BlinkIT Grocery Data'[Sales] )
        Avg Sales = AVERAGE('BlinkIT Grocery Data'[Sales])
        Avg rating = AVERAGE('BlinkIT Grocery Data'[Rating])
        No of items = COUNTROWS('BlinkIT Grocery Data') 
   
- Step 6 : While creating dashboard first  write the name of company.
- Step 7 : make a new parameter named Matrix which contain (Total sales , Average sales ,Average rating ,No of items). then make 4 kpi new cards and place it 
- Step 8 :Make sclicer of that Matrix. A donut chart of fat content, clustered chart of (Fat by outlet and Item type)  were also added to the report design area .
- Step 9 : Treemap for outlet size , Funnel for outlet location ,Area chart for outlet establishment and matrix  were used.
- Step 10 :The report was then published to Power BI Service.


# Snapshot of Dashboard (Power BI Service)

![dashboard_snapo]( ![Screenshot 2024-10-11 121423](https://github.com/user-attachments/assets/54762dc3-88e7-4af6-8a66-96671c96e27a))


# Insights

A single page report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;

 
