# Student-data-saver-and-viewer
In this i have hands on practiced AWS IAM ,dynamodb,lambda,API,s3 to store my html files
# Student Data CRUD App (AWS Lambda + DynamoDB + API Gateway)
A serverless web application that allows users to insert and retrieve student records using AWS Lambda, DynamoDB, and API Gateway. Built with simplicity and scalability in mind, this project demonstrates core cloud-native development skills including API design, CORS handling, and infrastructure documentation.

# Live Demo

# this is the overview of my project interface
---<img width="827" height="662" alt="Screenshot 2025-08-15 141134" src="https://github.com/user-attachments/assets/41b4f43c-6bf7-494b-8814-8f32a5b9b8b1" />
   
# After adding the input
<img width="830" height="581" alt="Screenshot 2025-08-15 141245" src="https://github.com/user-attachments/assets/ea698f7b-9a20-4799-859d-639f06148f65" />

# to preview all the data stored in the Cloud
<img width="827" height="662" alt="Screenshot 2025-08-15 141134" src="https://github.com/user-attachments/assets/207a3239-03b1-4997-904f-314c30e4d23a" />


# Used Services
- **Frontend**: HTML, JavaScript
- **Backend**: AWS Lambda (Node.js)

- **Database**: DynamoDB
- **API Gateway**: REST API with Lambda Proxy Integration
- **Deployment**: AWS Console (manual setup)


## 📦 Features

-  Insert student data via POST request
-  Retrieve all student records via GET request
-  CORS enabled for frontend integration
-  Clean JSON responses for easy parsing
-  Serverless architecture with minimal cost

---

## Real life application 
1.As i showed in the above image(demo) we can use it in School/college management systems
 for further upgradation we can use API and manage who and all can only upload student data and manage who have the authority to access the data.
2.Hospital management system (by changing the table heading we can store Patients name, age and their respective wards or departments)

# stpes 
1.create a iam role including policies

    1.AmazonDynamoDBFullAccess
    2.AWSLambda_FullAccess
    3.AWSLambdaBasicExecutionRole

2.Create two lambda functions 

   1.one lambda function to insert student values whenever thw save action get invoked it will store it into the data table
   2.Another lambda funtion to get student data from the table whenever the get student data action invokes

3.API gateway

   Next important step after making the lambda funtions we have to create API gate way for them with using respective GET,PUT options 
   after all of this we have to enable CORS

4 Dynamodb

  to store all of my data

5.S3

which include my html and javascript code also the api endpont should be included into my js


 
