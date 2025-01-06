# TextTools_PowerBI
Analytics Manager wants to better understand where our customers may be coming from, based on their email domains.
## Objective
Create a new colimn in the customer table that will allow for this to happen.
## Tools and Techniques
1. Duplicate the email address column and name it 'Domain Name'

2. In the new column, remove all text/characters except for the domain name.

3. Use transformations steps to clean up and capitalize the domain names.

4. Save & apply changes.
## Features and Insights 
## Workflow 
1. Create two new queries that connect to the PRODUCT CATERGORY LOOKUP and PRODUCT SUBCATEGORY LOOKUP.
   
3. Update these table names.
   
5. Make sure that the column headers have been promoted and that all data types are correct.
    
7. Add a new column to extract all characters before the '-' and product SKU and name it 'SkU type'. -> Add \column\ in PRODUCT LOOKUP query through \extracting\ "text before delimitor '-'". Notice that new columns are added on the far right of the table. Rename that extracted column 'SKU type'.
   
9. Update 'SKU Type' calculations to return all characters before the second '-' instead of the first '-'. Go to \Applied Steps\ on the right -> \gear icon\ of 'text before delimitor' -> \advnaced options\ -> 'number of delimiters to skip <1>' -> \ok\.
    
11. Replace '0' in 'ProductStyle' column with 'NA' by -> making sure \renanmed column\ is selected in \applied steps\ (otherwise query will break) -> click 'ProductStyle' -> \transform tab\'s \replace value\ '0' with 'NA'. Check drop down of 'ProductStyle' and notice that all '0' has been replaced.
    
13. Load all these changes into the data model by -> \home\ -> \close & apply\
## Screenshots of Dashboards 
## Results and Impact 
## Future Improvements 
