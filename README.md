			Data Cleaning and Transformation	
      
	1) Handling Missing Values:									
		• Check for missing values in the 'Price' column. How would you handle products with missing price information?	
    In Excel, I performed find and replace with "Unknown". 
    
		• If there are products with missing categories, propose a strategy to impute or deal with these missing values effectively.		
    In Power Query, using "conditional column" in the Add Column ribbon I gave the the following conditions if "category" "does not equal" to null then "category", 
    else if [Product Name] = "Backpack" then "Outdoor"
    else if [Product Name] = "Sneakers" then "Fashion"
    else if [Product Name] = "Coffee Maker" then "Kitchen"
    else if [Product Name] = "Fitness Tracker" then "Electronics"
    else "Unknown"
										
	2) Correcting Inconsistent Data:									
		• Identify any inconsistent text formats present in the "Product Name" column.
    Trimed, Cleaned and Capitalized the words
    
		• Identify any typos present in the "Category" column.
    Identified the typos
    
    
		• Use the find and replace function to standardize the text formats in the "Product Name" column and fix any typos or misspellings in the "Category" column.
    Trimed, Cleaned and Capitalized the words, and replaced "Electroni"  with "Electronics" using **Replace Values** in the Power Query
										
	3) Removing Duplicates:									
		• Identify any duplicate rows within the dataset based on the entirety of each row, and remove them if any.	
    Removed the duplicates, using **Remove rows** in Power Query
										
	4) Splitting and Merging Data:									
		• Split the "Product ID" column into two separate columns for " Manufacturing Date" and "Country Code". Remove unnecessary characters, if any.
    Splitted "Product ID" using **Split Coloumn ** and by delimiter "-"
    
		• Merge the "Brand Name" and "Product Name" columns into one column named "Product Brand".
    Merged " Brand Name" and "Product Name" column by **Merge Column** in Transform ribbon 
    
										
	5) Number Formatting:									
		• Format the data type of the "Price" column to currency format. 		
    Performed the currency formatting in the excel.
    
		• Format the "Manufacturing Date" column to display dates in the "DD-MM-YYYY " format. 
    Performed the date formatting in the excel.
    
										
	6) Conditional Formatting:									
		• Apply data bar or color scales conditional formatting in the "Price" column.	
    Applied data bar in the "Price Column". 
    
		• Create a custom rule for conditional formatting in the "Category" column to highlight cells where the category is "Electronics."
    Highlighted the "Electronics" in the category column 
										
										
<img width="1374" height="599" alt="image" src="https://github.com/user-attachments/assets/4d7a627c-8215-43a5-ab01-ad34d99bcd5f" />
