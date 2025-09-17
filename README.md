# Deploying a Web Application in the Cloud
This guide outlines the process of deploying a simple web application using a cloud service provider. Follow these steps to gain a fundamental understanding of cloud deployment, including setting up a virtual server, configuring a web application, and utilizing essential cloud services.

Project Overview

The aim is to provide a clear method for deploying a web application in the cloud through the following steps:

1. Setting Up a Virtual Server

        1.Log into the Management Console: Access the cloud service provider's management console.

        2.Launch Instance: Navigate to the dashboard and click "Launch Instance."

        3.Choose an AMI: Select an Amazon Machine Image (AMI), such as Amazon Linux 2.

        4.Select Instance Type: Choose an instance type, such as t2.micro (free tier eligible).

        5.Configure Security Groups: Allow HTTP (port 80) and SSH (port 22) access.

        6.Review and Launch: Launch the instance, creating or selecting an existing key pair for SSH access.

2. Uploading Application Files to Cloud Storage

        1.Access S3 Dashboard: Navigate to the S3 service dashboard.

        2.Create Storage Bucket: Create a new S3 bucket or choose an existing one.

        3.Upload Files: Upload your web application files to the S3 bucket.

3. Connecting to the Server with SSH

        1.Install SSH Client: Download and install an SSH client if not already installed (e.g., PuTTY).

        2.Convert Key Pair: Convert the .pem key pair file to a .ppk file using PuTTYgen.

3.Connect via SSH Client:

        Enter the public DNS or IP address of the EC2 instance in the SSH client.
        
        Configure the SSH client to use the key pair file.
         
        Connect to the instance and log in as ec2-user
4. Transferring Files from S3 to the Server

        1.Install AWS CLI: Install the AWS CLI on the EC2 instance.

        2.Copy Files: Use aws s3 cp commands to copy files from the S3 bucket to the EC2 instance.

5. Running the Web Application

        1.Navigate to Application Directory: Go to the directory containing your application files.

        2.Set Up Dependencies: Ensure all necessary dependencies and environment variables are configured.

        3.Start Application: Run the application using the relevant command (e.g., npm start, python app.py, etc.).

        4.Verify Deployment: Access the public IP address of the EC2 instance in a web browser to verify that the application is running.

Technologies Utilized

Amazon Web Services (AWS)

   EC2: For hosting the application.
   
   S3: For storing application files.
   
   PuTTY: For secure SSH connection.

   AWS CLI: For managing AWS services from the command line.


<img width="1911" height="773" alt="image" src="https://github.com/user-attachments/assets/474393f5-1ea5-42e4-8c36-e7e38ff81ae9" />



![WhatsApp Image 2025-09-17 at 15 29 02_997541d1](https://github.com/user-attachments/assets/2fbb0388-0ab0-4eb1-8fd0-64c37837ab13)



<img width="1919" height="775" alt="image" src="https://github.com/user-attachments/assets/4c598ddd-d83a-46eb-a2a2-f16f5832f8fc" />



<img width="1919" height="776" alt="image" src="https://github.com/user-attachments/assets/0f3c6fc0-6731-491e-b1f5-4e5631e29c48" />


<img width="1913" height="890" alt="image" src="https://github.com/user-attachments/assets/7f518b24-16de-4a1b-9dac-e6f86c1a9b42" />



