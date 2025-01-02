The Nashville Housing Data Cleaning project focused on transforming and standardizing a complex real estate dataset using PostgreSQL. The raw data presented several challenges including inconsistent date formats, non-standardized categorical values, merged address fields, duplicate entries, and null values across multiple columns. To address these issues, I first established a structured database schema with appropriately defined columns for housing sales data. I then implemented a series of SQL solutions to clean and standardize the data. This included converting sale dates to a consistent YYYY-MM-DD format, standardizing the 'SoldAsVacant' field from Y/N to Yes/No values, and cleaning ParcelIDs by removing non-numeric characters. One of the major improvements involved breaking down concatenated owner addresses into separate components (street, city, and state) using string manipulation functions, making the location data more accessible for analysis. I also developed a solution to handle missing property addresses by implementing a self-join strategy that populated null values using matching ParcelID information. To ensure data integrity, I created a backup table before removing duplicate records using window functions and Common Table Expressions (CTEs). The final result was a clean, standardized dataset ready for analysis, with properly formatted dates, standardized categorical values, separated address components, and no duplicate entries. This project showcases my proficiency in SQL data cleaning techniques, including the use of window functions, CTEs, regular expressions, string manipulation, and date formatting, while maintaining data integrity throughout the cleaning process.
Below is an image of the data before cleaning and after cleaning 
![Screenshot 2025-01-02 091005](https://github.com/user-attachments/assets/f88eea57-c96e-49d1-bf44-627c7bd52eed)
![Screenshot 2025-01-02 090914](https://github.com/user-attachments/assets/57d017e5-9ba6-473e-b1c3-6d814e080ab6)