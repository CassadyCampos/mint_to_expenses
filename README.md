# mint_to_expenses

### How to Run
1. Place exported Mint CSV files into the directory /transactions

2. (Optional) Modify any categories you'd like to filter out and not include in the end results
within mint_to_expenses_transform.py. 

2. 1. If running on a fresh machine, you may need to install python and make sure you have these packages installed
    pip install pandas
    pip install openpyxl

3. When you're ready run the script command
'python mint_to_expenses_transform.py'

- When entered you should receive output log responses of the converted files

4. Pretty much done! Look inside the directory /transformed to view the resulting spreadsheet

5. Import the file into Google Chrome and omit rows, change the ratio of the amount owed etc...


