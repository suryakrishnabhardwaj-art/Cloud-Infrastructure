# Cloud-Based Smart Parking Management System

A scalable, secure, and cloud-hosted parking management application that helps drivers check parking availability, reserve parking slots, and manage bookings in real time.

## Project Overview

Finding an available parking space in busy areas can waste time, increase fuel consumption, and contribute to traffic congestion. The **Cloud-Based Smart Parking Management System** addresses this problem through a web application that provides real-time parking availability and booking management.

The application is hosted on **Amazon EC2** instances behind an **Elastic Load Balancer**. An **EC2 Auto Scaling Group** automatically adds or removes instances based on demand. **Amazon DynamoDB** stores parking slot status, user bookings, and vehicle entry/exit details. Administrators can monitor occupancy and usage through a centralized dashboard.

## Objectives

- Allow users to view available parking slots in real time.
- Enable users to reserve a parking slot and manage their bookings.
- Maintain parking slot status and entry/exit details continuously.
- Provide administrators with a centralized view of parking occupancy and usage.
- Support changing traffic levels through load balancing and automatic scaling.
- Protect application resources through AWS network controls and identity permissions.
- Monitor application health and performance.

## Key Features

- **Live parking availability:** View the current status of parking slots.
- **Slot reservation:** Reserve an available parking slot through the web application.
- **Booking management:** Manage parking reservations.
- **Entry and exit tracking:** Store vehicle entry and exit details.
- **Admin dashboard:** Monitor parking occupancy and usage.
- **Scalable hosting:** Add or remove application instances automatically as demand changes.
- **Traffic distribution:** Distribute incoming application traffic across EC2 instances.
- **Monitoring:** Track system health and performance using Amazon CloudWatch.
- **Access protection:** Use VPC security groups and AWS IAM roles to control access.

## AWS Services Used

| AWS service | Purpose in this project |
|---|---|
| **Amazon EC2** | Hosts the parking application servers. |
| **Amazon EC2 Auto Scaling** | Automatically adds or removes EC2 instances according to demand. |
| **Elastic Load Balancing (ELB)** | Distributes incoming traffic across application instances. |
| **Amazon DynamoDB** | Stores parking slot information, user bookings, and entry/exit details. |
| **Amazon CloudWatch** | Collects metrics, monitors system health and performance, and supports scaling alarms. |
| **Amazon VPC** | Provides the network environment and security groups for the application. |
| **AWS IAM** | Manages access permissions and roles for AWS resources. |

## High-Level Architecture

```text
                         Users
                           |
                           v
                  Web Application
                           |
                           v
              Elastic Load Balancer (ELB)
                           |
                           v
             EC2 Auto Scaling Group
                  /             \
                 v               v
             EC2 Instance    EC2 Instance
                  \             /
                   \           /
                    v         v
                  Amazon DynamoDB
             (slots, bookings, entry/exit)

       Amazon CloudWatch: monitoring and scaling alarms
       Amazon VPC: network and security groups
       AWS IAM: access permissions and roles
```

## How the System Works

1. A user opens the web application to check parking availability.
2. The application retrieves the latest parking slot information from Amazon DynamoDB.
3. The user selects an available slot and makes a reservation.
4. Booking information and parking status are updated in DynamoDB.
5. Vehicle entry and exit details are stored to support occupancy tracking.
6. Administrators use the dashboard to monitor parking occupancy and usage.
7. Elastic Load Balancing distributes incoming requests across the available EC2 instances.
8. EC2 Auto Scaling adjusts the number of instances as demand changes.
9. Amazon CloudWatch monitors metrics and system performance and provides alarms used for scaling.
10. Amazon VPC security groups and AWS IAM roles help protect the application and its AWS resources.

## Security and Reliability

- **Network security:** Amazon VPC security groups help control network access.
- **Identity and permissions:** AWS IAM roles manage access to AWS resources.
- **Traffic management:** Elastic Load Balancing distributes requests across instances.
- **Elastic capacity:** EC2 Auto Scaling responds to changes in demand.
- **Operational monitoring:** Amazon CloudWatch tracks system health and performance.

## Expected Outcome

The expected outcome is a scalable, reliable, and secure parking solution that:

- Reduces the time drivers spend searching for parking.
- Improves the utilisation of available parking spaces.
- Provides users with real-time parking availability and booking management.
- Helps administrators monitor occupancy and usage.
- Demonstrates how AWS cloud services can support smart-city applications.

## Project Information

| Detail | Information |
|---|---|
| **Project title** | Cloud-Based Smart Parking Management System |
| **Course** | Cloud Infrastructure and Services |
| **Course code** | 25CS2206E |
| **Academic year** | 2026–2027 |
| **Team number** | 3 |
| **Section** | 12 |
| **Guide** | Mrs. Divya Priya Degala, Associate Professor, CSIT |

### Team Members

| Name | Roll number |
|---|---|
| V. Bhardwaj | 2520090182 |
| P. Uday | 2520090089 |
| A. Chaitanya | 2520090094 |

## Repository Contents

This repository contains the project source code, configuration, and supporting documentation as they are added during development.

> **Note:** The implementation language, web framework, repository folder structure, and deployment commands are not specified in the project abstract. Add the exact setup and run instructions here once those implementation details are finalized.

## Future Enhancements

The following are possible extensions and are not stated as completed features in the project abstract:

- Integrate sensors or IoT devices for automated vehicle detection.
- Add payment integration for paid parking facilities.
- Provide reservation notifications and reminders.
- Add analytics for parking demand and usage trends.

---

**Project:** Cloud-Based Smart Parking Management System  
**Course:** Cloud Infrastructure and Services (25CS2206E)
