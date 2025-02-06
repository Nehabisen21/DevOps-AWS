# AWS IAM

## What is IAM? How Identity and Access Management Works?

  - AWS(Amazon Web Services) will allow you to maintain the fine-grained permissions to the AWS account and the services provided by Amazon Cloud.
  - You can manage the permissions to the individual users or you can manage the permissions to certain users as groups and roles will help you to manage the permissions to the resources.

---
## How to create IAM user and attach required permission to the user

- Login to AWS <a href="https://signin.aws.amazon.com/signin?redirect_uri=https%3A%2F%2Fus-east-1.console.aws.amazon.com%2Fiam%2Fhome%3FhashArgs%3D%2523%252Fhome%26isauthcode%3Dtrue%26oauthStart%3D1738838004557%26region%3Dus-east-1%26state%3DhashArgsFromTB_us-east-1_1fd333b726da4261&client_id=arn%3Aaws%3Asignin%3A%3A%3Aconsole%2Fiamv2&forceMobileApp=0&code_challenge=1UaqaA3tSgCTr_IdOVvB4OYH51LY8cEckDKBCuHi1Gc&code_challenge_method=SHA-256">console</a>
![image](https://github.com/user-attachments/assets/f033c8d0-4316-497c-aa0d-c16fc6014dd4)

- After login, go to the search bar of AWS and search for IAM and click on it.
  
![image](https://github.com/user-attachments/assets/3e4c2e4f-7e23-4356-aa67-9bb3d8dd067c)

- Now, let's create a user, go to IAM and on the left sidebar click on users, as shown in the below screenshot

![image](https://github.com/user-attachments/assets/7cb6415b-1cb0-4104-bf9c-cfa4600222fa)

- Now, click on **create user**

  - Specify username, in this case we will use aws-admin as a user name and click on next.

  ![image](https://github.com/user-attachments/assets/cc177463-415e-4db7-8490-a071dde2020d)

  - Now, we need to assign permission as per the user requirement, as we are creating **aws-admin** user, we will provide adminisitrator access, so click on **attach policy directly** and search for **AdministratorAccess**.
 
  ![image](https://github.com/user-attachments/assets/1c2d3a14-04bf-4102-af6f-9cbc5f87fb0e)
 
  - Now, click on next and review your details and click on **create user**

  ![image](https://github.com/user-attachments/assets/9ad22f77-7118-4d8f-a801-7c341c301328)

  - Congratulations, you have successfully create an IAM user on AWS.
  
