# AWS IAM

## What is IAM? How Identity and Access Management Works?

  - AWS(Amazon Web Services) will allow you to maintain the fine-grained permissions to the AWS account and the services provided by Amazon Cloud.
  - You can manage the permissions to the individual users or you can manage the permissions to certain users as groups and roles will help you to manage the permissions to the resources.

---
## How to create IAM user and attach required permission to the user


- After login, go to the search bar of AWS and search for IAM and click on it.
  

- Now, let's create a user, go to IAM and on the left sidebar click on users, as shown in the below screenshot


- Now, click on **create user**

  - Specify username, in this case we will use aws-admin as a user name and click on next.

  ![image](https://github.com/user-attachments/assets/cc177463-415e-4db7-8490-a071dde2020d)

  - Now, we need to assign permission as per the user requirement, as we are creating **aws-admin** user, we will provide adminisitrator access, so click on **attach policy directly** and search for **AdministratorAccess**.
 
  ![image](https://github.com/user-attachments/assets/1c2d3a14-04bf-4102-af6f-9cbc5f87fb0e)
 
  - Now, click on next and review your details and click on **create user**

  ![image](https://github.com/user-attachments/assets/9ad22f77-7118-4d8f-a801-7c341c301328)

  - Congratulations, you have successfully create an IAM user on AWS.
  
