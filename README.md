# Aws-Blue-Green-Deployment
AWS Blue-Green Deployment with Canary Traffic Shifting
# AWS Blue-Green Deployment with Canary Traffic Shifting

## Project Overview

This project demonstrates Blue-Green Deployment on AWS using an Application Load Balancer (ALB).

Two EC2 instances were used:

- Blue Server – Version 1
- Green Server – Version 2

Apache HTTP Server was installed on both EC2 instances to host the web pages.

## AWS Services Used

- Amazon VPC
- Amazon EC2
- Application Load Balancer
- Target Groups
- Security Groups
- Internet Gateway
- Route Table
- Apache HTTP Server

## Deployment Process

1. Created a VPC with CIDR `10.0.0.0/16`.
2. Created two public subnets.
3. Configured Internet Gateway and Route Table.
4. Created a Security Group with HTTP access.
5. Launched Blue EC2 server.
6. Installed Apache and configured the Blue web page.
7. Launched Green EC2 server.
8. Installed Apache and configured the Green web page.
9. Created separate Target Groups for Blue and Green servers.
10. Created an Application Load Balancer.
11. Configured Canary traffic shifting.
12. Tested the deployment.
13. Finally shifted 100% traffic to the Green server.

## Canary Traffic Shifting

Initial traffic distribution:

- Blue: 80%
- Green: 20%

Final traffic distribution:

- Blue: 0%
- Green: 100%

## Blue Version

`VERSION 1 (BLUE)`

## Green Version

`VERSION 2 (GREEN)`

## Result

The Blue-Green deployment was successfully implemented using AWS Application Load Balancer.

Canary traffic shifting was tested successfully, and finally 100% of the traffic was shifted to the Green version.

## Learning Outcomes

- AWS VPC configuration
- EC2 instance deployment
- Apache web server configuration
- Target Group configuration
- Application Load Balancer configuration
- Canary traffic shifting
- Blue-Green deployment
