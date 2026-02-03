Here is a clean and professional **README.md** rewritten and elaborated so you can directly paste it into your project 👇

---

# AWS EC2 Manual Launch & Terraform Automation Project

## Project Overview

This project demonstrates two approaches to launching an **Amazon EC2 instance**:

1. **Manual Method** – Creating an EC2 instance using the AWS Management Console.
2. **Automation Method** – Creating an EC2 instance using **Terraform (Infrastructure as Code)**.

The objective is to understand the difference between manual provisioning and automated infrastructure deployment.

---

## Objective

* Learn the fundamentals of AWS EC2.
* Understand manual cloud resource creation.
* Practice Infrastructure as Code using Terraform.
* Compare manual vs automated deployment methods.

---

## Part 1 – Manual EC2 Instance Creation

In this section, the EC2 instance was launched manually through the AWS Console.

### Steps Performed

1. Logged into the AWS Management Console.
2. Navigated to the **EC2 Dashboard**.
3. Clicked on **Launch Instance**.
4. Selected **Amazon Linux AMI**.
5. Chose instance type **t3.micro** (Free Tier eligible).
6. Configured **Security Group**:

   * Allowed **SSH (Port 22)** – for remote access.
   * Allowed **HTTP (Port 80)** – for web traffic.
7. Reviewed configuration and launched the instance.
8. Verified that the instance state changed to **Running**.

### Outcome

* Successfully created and accessed a virtual server.
* Gained hands-on experience with AWS Console navigation and configuration.

---

## Part 2 – EC2 Instance Creation Using Terraform

In this section, the same EC2 infrastructure was created using Terraform automation.

### Prerequisites

* AWS Account
* Terraform installed
* AWS CLI installed
* Configured AWS credentials using:

```
aws configure
```

---

### Steps Performed

1. Installed **Terraform** on the local machine.
2. Installed **AWS CLI** and configured credentials.
3. Created a project directory.
4. Created a file named `main.tf`.
5. Defined AWS provider and EC2 resource configuration.
6. Ran the following Terraform commands:

#### Initialize Terraform

```
terraform init
```

#### Preview Changes

```
terraform plan
```

#### Apply Configuration

```
terraform apply
```

7. Confirmed resource creation in AWS Console.
8. Verified that the EC2 instance was successfully launched.

---

## Key Learnings

### Manual Method

* Good for beginners.
* Helps understand AWS interface.
* Time-consuming for large environments.
* Prone to human errors.

### Terraform Method

* Faster and repeatable.
* Infrastructure can be version-controlled.
* Reduces manual mistakes.
* Industry-standard DevOps practice.

---

## Folder Structure

```
project-root/
│
├── main.tf
├── screenshots/
│   ├── manual-ec2.png
│   ├── terraform-init.png
│   ├── terraform-apply.png
│
└── README.md
```

---

## Screenshots

All relevant screenshots demonstrating both manual and Terraform steps are available in the **/screenshots** folder.

---

## Conclusion

This project highlights the transition from **manual cloud management** to **Infrastructure as Code (IaC)** using Terraform.
Understanding both approaches provides a strong foundation for **Cloud Engineering and DevOps roles**.

---

## Future Improvements

* Add VPC and Subnet creation via Terraform.
* Use Terraform variables and modules.
* Implement remote state storage using S3.
* Add automated security group rules.

---

**Author:** *Your Name*
**Technologies Used:** AWS EC2, Terraform, AWS CLI, Linux

---
