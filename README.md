Project Title:
Deploying a Public Amazon EC2 Instance within a Custom VPC on AWS

Objective:

To design, implement, and configure a secure, scalable infrastructure in AWS by launching an EC2 instance within a Virtual Private Cloud (VPC), ensuring controlled internet access through proper subnetting, route table configuration, and the use of an Internet Gateway (IGW). This environment serves as a foundational setup for hosting web applications, development servers, or remote-accessible services.

Architecture:

![image](https://github.com/user-attachments/assets/15f18a21-0ee9-45b9-ba1d-07727e182740)

Architecture Overview:

The implemented architecture includes the following components:
  -  Region: A specific geographical area where AWS resources are hosted.
  -  VPC (Virtual Private Cloud): A logically isolated section of AWS where resources are launched.
  -  Subnet: A segment of the VPC IP address range used to group and isolate resources.
  -  Security Group: A virtual firewall controlling inbound and outbound traffic for the EC2 instance.
  -  EC2 Instance: A virtual server used to host applications or services.
  -  Internet Gateway (IG): Enables internet access for instances in the VPC.
  -  Route Table: Contains routing rules directing subnet traffic to the IGW for internet access.

Security Considerations:

  -  Limited inbound SSH access to specific IP ranges.
  -  Used a key pair for secure EC2 instance access.
  -  Outbound internet access is controlled via the route table and security group rules.

Use Cases:

  - Hosting a website or web application.
  - Creating a development or testing environment.
  - Remote-access server for administrative tasks.

