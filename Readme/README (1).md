# Cloud-Based Smart Parking Management System

## Project Information

| Detail | Information |
|---|---|
| Course | Cloud Infrastructure and Services |
| Course Code | 25CS2206E |
| Academic Year | 2026–2027 |
| Team Number | 4 |
| Section | 12 |
| Institution | KLH University, Bowrampet, Hyderabad, Telangana, India |

## Project Description

Finding a free parking space in busy areas wastes time, increases fuel consumption, and contributes to traffic congestion. The **Cloud-Based Smart Parking Management System** is designed to help users check parking availability, reserve a parking slot, and manage bookings in real time through a web application.

The application is hosted on **Amazon EC2 instances** behind an **Elastic Load Balancer**. An **EC2 Auto Scaling Group** automatically adds or removes instances according to demand, helping the application remain responsive during peak hours and cost-efficient during periods of lower demand.

Parking-slot status, user bookings, and vehicle entry and exit details are stored in **Amazon DynamoDB** and updated continuously. Drivers can view parking availability, while administrators can use a centralized dashboard to monitor parking occupancy and usage.

The solution also uses **Amazon CloudWatch** to monitor system health and performance. **Amazon VPC security groups** and **AWS IAM roles** help secure the application environment and control access to cloud resources.

## Problem Statement

In busy areas, drivers often spend considerable time searching for vacant parking spaces. This increases fuel consumption and contributes to traffic congestion. A centralized, cloud-hosted parking solution is needed to show parking availability, support slot reservations, manage bookings, and help administrators monitor parking usage.

## Objectives

- Allow users to check parking-slot availability in real time.
- Enable users to reserve parking slots and manage their bookings.
- Maintain parking-slot status, booking information, and entry and exit details.
- Provide administrators with a dashboard to monitor occupancy and usage.
- Host the application on AWS infrastructure for scalability and reliability.
- Use monitoring and access-control services to support system health and security.
- Manage changing user demand efficiently through automatic scaling and load distribution.

## Key Features

- **Real-time parking availability:** Users can check which parking slots are available.
- **Slot reservation:** Users can reserve a parking slot through the web application.
- **Booking management:** Users can manage their parking bookings.
- **Entry and exit tracking:** The system maintains vehicle entry and exit details.
- **Administrator dashboard:** Administrators can monitor parking occupancy and usage.
- **Load balancing:** Elastic Load Balancing distributes incoming application traffic across EC2 instances.
- **Automatic scaling:** EC2 Auto Scaling adjusts the number of application instances based on demand.
- **Cloud monitoring:** Amazon CloudWatch monitors system health and performance.
- **Cloud security:** Amazon VPC security groups and AWS IAM roles help protect resources and manage permissions.

## System Architecture

The project uses the following high-level cloud architecture:

**Users → Web Application → Elastic Load Balancer → Amazon EC2 Auto Scaling Group → Amazon DynamoDB**

Supporting AWS services:
- **Amazon CloudWatch:** Monitors application and infrastructure performance and supports scaling alarms.
- **Amazon VPC:** Provides the cloud network environment and security groups.
- **AWS IAM:** Manages roles and permissions for access to AWS resources.

## Working Process

1. A user opens the smart parking web application.
2. The user checks the current parking-slot availability.
3. The user selects and reserves an available slot.
4. The application stores and updates parking-slot status and booking information in Amazon DynamoDB.
5. Vehicle entry and exit details are maintained by the system.
6. The administrator views parking occupancy and usage through a centralized dashboard.
7. Incoming application traffic is distributed by Elastic Load Balancing across the available EC2 instances.
8. EC2 Auto Scaling adds or removes instances according to demand.
9. Amazon CloudWatch monitors system health and performance, while VPC security groups and IAM roles help protect cloud resources.

## AWS Services Used

| AWS Service | Purpose in the Project |
|---|---|
| Amazon EC2 | Hosts the parking application servers. |
| Amazon EC2 Auto Scaling | Automatically adds or removes EC2 instances based on demand. |
| Elastic Load Balancing | Distributes incoming traffic across application instances. |
| Amazon DynamoDB | Stores parking-slot status, booking data, and related records. |
| Amazon CloudWatch | Collects metrics and supports monitoring and scaling alarms. |
| Amazon VPC | Provides the network environment and security groups. |
| AWS IAM | Manages access permissions and roles for AWS resources. |

## Expected Outcome

The expected outcome is a scalable, reliable, and secure smart parking solution. The system aims to reduce the time drivers spend searching for parking, improve the utilization of available parking spaces, and provide administrators with a centralized view of parking occupancy and usage. The project demonstrates how AWS cloud services can support smart-city applications.

## Future Scope

- Extend the system to support multiple parking locations.
- Enhance parking analytics and generate usage reports.
- Add notifications for booking confirmations and parking updates.
- Improve the user and administrator dashboard based on project requirements.
- Explore additional integrations for smart-city parking management.

## Team Details

| S. No. | Team Member | Roll Number |
|---|---|---|
| 1 | V. Bhardwaj | 2520090182 |
| 2 | P. Uday | 2520090089 |
| 3 | A. Chaitanya | 2520090094 |

**Team Number:** 4  
**Section:** 12

## Project Guide

**Mrs. Divya Priya Degala**  
Associate Professor, CSIT

## Institution

**KLH University**  
Bowrampet, Hyderabad – 500043, Telangana, India.

## Course Details

**Course:** Cloud Infrastructure and Services  
**Course Code:** 25CS2206E  
**Academic Year:** 2026–2027
