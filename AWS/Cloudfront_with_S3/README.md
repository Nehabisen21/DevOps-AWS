# What is CloudFront?

- Amazon CloudFront is a Content Delivery Network (CDN) service that securely delivers data, videos, applications, 
and APIs to users globally with low latency and high transfer speeds.
- It caches content at edge locations worldwide, reducing the load on the origin server and improving performance.
- CloudFront integrates with AWS services like S3, EC2, and Lambda@Edge to enhance security and scalability. 
- It also supports DDoS protection, SSL/TLS encryption, and access control for secure content delivery.

![image](https://github.com/user-attachments/assets/a31c6f23-49d0-46e8-b545-1e23dcceef6e)

##   Now, We will intergrate cloudfront with S3 Bucket


  ![cloudfront_draw](https://github.com/user-attachments/assets/84f2b596-73de-42ae-8475-d4e505085c3d)


- Firstly we create S3 bucket

  - Then, upload objects in buckets, I used code files

  - Go to the permission setting in S3 and Block public access i.e off
 
  - then go to bucket policy and add below policy 

    ![image](https://github.com/user-attachments/assets/6d7d70b9-49aa-46c0-ad12-2e9292140dea)

    - Now go to properties of s3 bucket and enable static website hosting

       ![cloudfront5_s3](https://github.com/user-attachments/assets/26085641-c494-4a64-8314-90edab9b51fa)

  - Add index.html in index document (must) and click to save changes.

---

## Now, create cloudfront

- Select origin domain, our origin domain is s3 so It will show s3 bucket name.
- origin domain would be from load balancer, API, EC2 instance

- select origin access

  ![cloudfront3_s3](https://github.com/user-attachments/assets/45d08b11-8b17-4c78-9c8d-dada9055a2ef)

  - after selecting the OAC  (more  secure for s3) it will provide bucket policy which we have to paste in bucket policy

  - Now Copy Distribution domain name and paste in new tab and then hit

     ![image](https://github.com/user-attachments/assets/a360bb92-b2be-4ae2-9bb2-9deb398376c9)

    ## You will see the website which we stored in s3 bucket


  ![cloudfront6_s3](https://github.com/user-attachments/assets/23e1d6bc-1cca-455e-ae69-9092d3d2b3f7)

   ## Congratulations, You configure the s3 bucket with cloudfront     




