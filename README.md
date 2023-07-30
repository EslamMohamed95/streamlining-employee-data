# Employee Data Structuring
### Overview
As the first data practitioner at a small business experiencing exponential growth, your first mission is to structure the human resources data. The data is currently scattered across teams and files and comes in various formats, including Excel files, CSVs, JSON files, and SQL databases. The company needs more structured processes, guidelines, and standards for data management.

The Head of People Operations wants to have a general view, gathering all available information about a specific employee, in a single reference file. Your task is to merge and consolidate all relevant employee data into a single pandas DataFrame and export it to a CSV file.

### Loading Data from CSV and Excel Files
To begin, you started by loading the company office addresses from two separate files into pandas DataFrames:

office_addresses.csv: Contains information about company office addresses.
employee_information.xlsx: Holds employee addresses and emergency contacts. The second sheet in this file, titled "emergency_contacts," needed some additional data cleaning as the header was removed.
Loading Employee Data from JSON Files
Next, you loaded employee role information, including titles, monthly salaries, and teams, from a JSON file titled "employee_roles.json." This file is structured as a Python dictionary with employee IDs as keys and corresponding role information as values.

Merging Several DataFrames into One
With individual DataFrames for office addresses, employee addresses, emergency contacts, and employee roles, you merged them to create a comprehensive DataFrame named df_employees. This unique DataFrame allows access to all employee data in a single view, enabling better data management.

### Editing Column Names
To improve the DataFrame's readability and consistency, you renamed some columns as per the request from People Ops. Duplicates and irrelevant columns were dropped, and the columns were reordered for better organization.

### Polishing the DataFrame
In the last-minute request, you performed some final touches to polish the DataFrame before exporting it:

Ensured all street numbers are in integer format.
Changed the DataFrame index to the actual employee ID.
Added a new column, "status," indicating whether an employee is "On-site" or "Remote" based on the presence of office information.
Saving Your Work
Finally, you saved the structured employee data into a CSV file named "employee_data.csv." This file serves as a reference for People Ops and lays the foundation for further data analysis and management.

As the data practitioner, you have successfully organized and consolidated scattered employee data, creating a more structured and streamlined data management process for the company. This file will be instrumental in making informed decisions and implementing data-driven strategies moving forward.
