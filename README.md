# mint_to_expenses

This app was migrated to AWS so I can run it on a monthly schedule instead of manually. 

### How to update
Ensure AWS CLI and Docker are installed on machine

* This project runs as a Lambda Function using a docker image from ECR

Make sure aws confiure is done, probably you're using a IAM user with an access key, secrets file might be saved by you somewhere secretly lol

In AWS Console open up the ECR repo and use the push commands to upload to the ECR instance


When it's done uploading, update the Lambda function to reference the latest version

Test the lambda function that it's working properly.




# Cant do this anymore
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


