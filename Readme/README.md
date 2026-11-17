# Cloud-Based Application Performance Benchmarking and Auto Scaling Evaluation

<p align="center">
  <strong>Cloud Infrastructure and Services (25CS2206E)</strong><br>
  Academic Year 2026–2027
</p>

---

## Project Overview

Cloud-based applications must maintain consistent performance under changing user demand while controlling infrastructure costs.

This project focuses on benchmarking a web application hosted on Amazon Web Services (AWS) and evaluating how effectively Auto Scaling responds to varying workloads.

A sample application will be deployed on Amazon EC2 instances behind an Elastic Load Balancer. An Auto Scaling Group will be configured with scaling policies based on CPU utilisation.

Different traffic patterns will be generated to evaluate application performance, resource utilisation, scaling behaviour and cost efficiency.

## Objectives

- Benchmark application performance under different workloads.
- Evaluate AWS Auto Scaling behaviour.
- Compare fixed-capacity and auto-scaled environments.
- Measure response time, throughput and error rate.
- Monitor CPU and resource utilisation.
- Analyse scaling delay and infrastructure cost efficiency.

## AWS Services Used

| AWS Service | Purpose |
|---|---|
| Amazon EC2 | Hosts application servers |
| EC2 Auto Scaling | Automatically adjusts instance capacity |
| Elastic Load Balancing | Distributes incoming traffic |
| Amazon CloudWatch | Monitors performance metrics |
| Amazon VPC | Provides network infrastructure |
| AWS IAM | Manages access permissions |

## Proposed Architecture

```text
              Users
                |
                v
        Load Testing Tool
                |
                v
    Elastic Load Balancer
                |
                v
       Auto Scaling Group
                |
        +-------+-------+
        |               |
        v               v
     EC2 Instance    EC2 Instance
        |               |
        +-------+-------+
                |
                v
        Amazon CloudWatch
         (Monitoring)
```

## Implementation Methodology

1. Deploy a sample web application on Amazon EC2.
2. Configure an Elastic Load Balancer.
3. Create an Auto Scaling Group.
4. Configure CPU-based scaling policies.
5. Generate different workloads using load-testing tools.
6. Monitor performance using Amazon CloudWatch.
7. Compare fixed-capacity and auto-scaled environments.

### Workload Scenarios

- Steady traffic
- Gradually increasing traffic
- Sudden traffic spikes

## Performance Evaluation Metrics

- Response Time
- Throughput
- Error Rate
- CPU Utilisation
- Scaling Delay
- Infrastructure Cost

## Expected Outcomes

- Understanding application performance under varying workloads.
- Evaluation of automatic scaling behaviour.
- Analysis of application stability during peak demand.
- Identification of suitable scaling policies and thresholds.
- Understanding the relationship between performance and cloud infrastructure costs.

## Team Details

**Team Number:** 4  
**Section:** 12

| Student Name | Roll Number |
|---|---|
| V. Bhardwaj | 2520090182 |
| P. Uday | 2520090089 |
| A. Chaitanya | 2520090094 |

## Project Guide & Course Instructor

**Mrs. Divya Priya Degala**  
Associate Professor, CSIT

## Repository Information

**GitHub Repository:**  
https://github.com/suryakrishnabhardwaj-art/Cloud-Infrastructure

---

<p align="center">
  <strong>Cloud Infrastructure and Services</strong><br>
  Team 4 | Section 12
</p>
