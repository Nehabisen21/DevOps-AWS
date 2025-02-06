  # CloudFront with Application Load Balancer

  ## Application Load Balancer 

 - For crearting load balancer firstly we need to create EC2 instance in which we will deploy our nginx server
 - For creating instances we need following configuration
     - name and tag
     - AMI
     - instance type
     - keypair
     - rest of configuration set default


  ![image](https://github.com/user-attachments/assets/aa282c5f-c742-416e-90a8-4811bdee307e)
  
  ![image](https://github.com/user-attachments/assets/d343b124-ddf1-4812-a902-796da1998f35)
  
  ![image](https://github.com/user-attachments/assets/44923934-5215-437c-8af4-ed8a51e21739)

  - Then click to launch instance and your ec2 instance is created
  - after creating connect that instance
  - install nginx instance

 
   ![image](https://github.com/user-attachments/assets/b9f80f49-d0bf-4a2e-8374-358d3a628d46)

    - after installation start and enable nginx
      - systemctl start nginx
      - systemctl enable nginx

   ![image](https://github.com/user-attachments/assets/34aae96a-1066-4668-b816-87c64d9c65f1)

   - after this go to security of instance and allow port no 80 for nginx so, that we can access the nginx

   ![image](https://github.com/user-attachments/assets/6e732785-d4f4-40fe-bfba-0c10048ad76f)

   - Now, copy public IP of your instance and paste in new tab and hit it, You get the nginx home page
   - if you want to edit nginx home page for that you need to configure index.html file in which we can add code

   ![image](https://github.com/user-attachments/assets/ba0e6e64-402e-4216-ac58-b7b74c99a439)

   ___

   ## Setup of Application load balancer

   - First thing to do while creating ALB is to create target group which is attach to our instance

      ![image](https://github.com/user-attachments/assets/ea64fa11-664f-4a4a-ad9d-6b2350b9b2bf)
     
      ![image](https://github.com/user-attachments/assets/259d25de-0364-4cd3-9544-416300bc68fa)


   - keep rest of the configuration as it is
      
     
      ![image](https://github.com/user-attachments/assets/0bbd595a-f765-4724-ace6-5f80243406b0)
     
      ![image](https://github.com/user-attachments/assets/1a2f0865-4e63-43a7-a526-7538449e8dcf)
     
      ![image](https://github.com/user-attachments/assets/1c1b10ac-99e5-4ce6-bd18-3f28083394a1)


     - our target group is ready
     - Now, we will go to Load balancer
     
     ![image](https://github.com/user-attachments/assets/d00a1f8e-cbe5-49c8-83ca-34967ff1370a)

     ![image](https://github.com/user-attachments/assets/9e9660f9-d29d-4a0c-a6c8-2e71d822a54c)

     - click on application load balancer
  
     ![image](https://github.com/user-attachments/assets/0f1478aa-fdb6-4b87-b56d-503225538452)

     ![image](https://github.com/user-attachments/assets/61b754f5-ec7e-41d8-aa44-99ea5f4bbde3)

     - click on all availability zones
     - then select our target group which we created just before it

     ![image](https://github.com/user-attachments/assets/93f90a39-c8f5-4621-b13d-cffbc312a43f)

     ![image](https://github.com/user-attachments/assets/e936c2ae-ebff-415b-b96a-77782e574d73)

     ![image](https://github.com/user-attachments/assets/da6561f3-08ce-42fc-9dc6-ef692d3a82d4)


     Yeahh! Your Application Load Balancer is ready

     - After activation of ALB
     - copy DNS name of ALB
       
  ![image](https://github.com/user-attachments/assets/dd5d1af3-8562-4981-b603-a2dff3a5027b)

       
  - paste it in new tab 

  
  ![image](https://github.com/user-attachments/assets/23f0e558-36b5-44af-82e6-f50900a75360)

   ## you will get your nginx home page which is running in your instance

  ---
  # CloudFront with ALB

  ![image](https://github.com/user-attachments/assets/a01a9f20-7776-4552-a584-ea387ebee321)
 
   ![image](https://github.com/user-attachments/assets/136ea660-4261-455a-8c97-730c04d25bd3)

   - cloudfront take time to get enable

   - copy distribution domain name


   ![image](https://github.com/user-attachments/assets/161f88ee-6a2e-4416-882c-8b4eac7d71e7)


   ## Here is your output from cloudfront

   ![image](https://github.com/user-attachments/assets/f776093b-1ac4-415a-8a7d-c0b56cfc18ab)

    



        
   



     






   






   
   
