CODE:KENTUCKY CAPSTONE PROJECT

# INTRO/OVERVIEW
Korean Medical Records/History from 2013 & 2023
The primary goal of the project is to look for differences between 2013 and 2023 in relation to utlization of mental health services.

# Project Setup Instructions

Steps to run this project:

The requirements to run this project are included in the 'Requirements.txt' folder. I created this project in a Jupyter notebook using Python (3.13.3) in a virtual environment.

1. Clone the repository
2. Navigate to the cloned directory
3. Set up a virtual environment & activate it

   | Command    | Linux/Mac                       | GitBash                         |
   | :--------- | :------------------------------ | :------------------------------ |
   | Create     | Python3 -m venv venv            | Python -m venv venv             |
   | Activate   | Source venv/bin/activate        | Source venv/Scripts/activate    |
   | Install    | Pip install -r requirements.txt | Pip install -r requirements.txt |
   | Deactivate | deactivate                      | deactivate                      |
5. Install the required packages by running 'pip install -r requirements.txt'
6. Run the Capstone.ipynb file
7. When you’re done, deactivate the virtual environment by entering ‘deactivate’ in your terminal


# TECHNOLOGIES/FEATURES USED
- Python is the main programming language for data analysis and scripting
- Chardet is used for detection of file encoding for robust data import
- PANDAS is used for data manipulation and analysis, including DataFrame operations
- Jupyter Notebook is used for coding & documentation
- Matplotlib is used for data visualization and plotting
- SQLite3 is used for SQL database for storing and querying large datasets


# ABOUT DATA

## DATA SOURCE

Description from [DATA.GO.KR:](https://www.data.go.kr/en/data/15007115/fileData.do)

“Medical history information is data consisting of basic information (gender, age group, city/province code, etc.) and medical history (medical department code, main disease code, number of treatment days, total prescription days, etc.) for 1 million patients in each year who have a medical history from a medical institution (hospital/clinic, etc.) among the National Health Insurance subscribers. For descriptions of codes for each item in the file, please refer to the 'Medical History Information User Manual'.”

DATA from 2013 & 2023 are used for this project.

## DATA SUMMARY

## DATA DICTIONARY
see Data Dictionary.ipynb file