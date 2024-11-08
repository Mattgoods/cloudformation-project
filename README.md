# 🚀 AWS Cloud Infrastructure with CloudFormation

### A scalable, secure, and modular AWS infrastructure built with Infrastructure as Code (IaC) 🛠️

---

## 📖 Overview
This project demonstrates a real-world cloud infrastructure setup using **AWS CloudFormation** to deploy a **Virtual Private Cloud (VPC)**, **EC2 instances**, **RDS database**, and associated security components. Designed to be secure, scalable, and cost-efficient, this infrastructure serves as a foundation for various applications, from e-commerce sites to data-driven web services, making it a valuable project for cloud engineers and architects.

## ✨ Key Features
- **Automated Deployment** 📈: All resources are provisioned using CloudFormation, allowing for quick, reliable, and repeatable deployments.
- **Networking & Security** 🔒: Includes public and private subnets, security groups, and IAM roles, following AWS best practices for network segmentation and access control.
- **Scalability** 🌐: Easily extendable to support additional EC2 instances, Auto Scaling, and more complex application architectures.
- **Cost Optimization** 💸: Configured to use cost-effective resources and isolate public-facing resources from sensitive data.

## 📂 Project Structure
```
.
├── templates/
│   └── cloud_infrastructure.yaml   # CloudFormation template defining the full AWS infrastructure
├── docs/
│   └── architecture_diagram.png    # Architecture diagram of the infrastructure setup (optional)
└── README.md                       # Project overview and setup instructions
```

## 🧱 Infrastructure Components

### 1. **VPC with Public and Private Subnets** 🌐
   - Custom **VPC** with a defined IP range, enabling control over network traffic.
   - **Public subnet**: Hosts an EC2 instance accessible from the internet.
   - **Private subnet**: Houses the RDS database, isolated from direct public access.

### 2. **EC2 Instance for Web Server** 🖥️
   - Configured with **security groups** to allow only HTTP and SSH access.
   - Automated setup using **User Data scripts** to install a web server, demonstrating automation and efficient deployment.

### 3. **RDS Database (e.g., MySQL) in Private Subnet** 📊
   - Database isolated in a private subnet to secure sensitive data.
   - Configured to allow access only from the EC2 instance, ensuring controlled connectivity.

### 4. **IAM Roles & Security Groups** 🔐
   - **IAM roles** provide granular permissions for resources, following the principle of least privilege.
   - **Security groups** restrict access based on specific IP ranges and ports, ensuring secure traffic flow within the environment.

## 💼 Real-World Applications
This infrastructure setup is ideal for a variety of use cases, including:
- **E-commerce Platforms** 🛒: Securely handle customer data, order processing, and inventory management.
- **Content Management Systems (CMS)** 📝: Host media and blog content with protected storage for articles and user data.
- **Internal Business Applications** 📊: Deploy intranet sites, data processing tools, and reporting platforms with secure data isolation.

## 🚀 Deployment

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/aws-cloud-infrastructure.git
   cd aws-cloud-infrastructure
   ```

2. **Modify Parameters** (if needed):
   - Open `cloud_infrastructure.yaml` and adjust parameters like CIDR ranges, instance types, or database configurations based on your requirements.

3. **Deploy with CloudFormation**:
   - Go to the [AWS CloudFormation Console](https://console.aws.amazon.com/cloudformation) and select **Create Stack**.
   - Upload the `cloud_infrastructure.yaml` file and follow the prompts to deploy the stack.

4. **View Outputs**:
   - Once the stack is deployed, view the Outputs section in CloudFormation to retrieve important details like EC2 public IP, VPC ID, and RDS endpoint.

## 🔮 Future Enhancements
- **Load Balancer and Auto Scaling**: Add a load balancer to distribute traffic and enable Auto Scaling for high availability.
- **CloudWatch Integration** 📊: Configure CloudWatch for monitoring and alerting to keep track of resource health and performance.
- **Multi-AZ RDS Setup** 🌍: Increase database reliability by enabling Multi-AZ replication for RDS.

## 📚 Learning Outcomes
This project demonstrates essential skills for cloud infrastructure management, including:
- **Infrastructure as Code (IaC)** 🛠️: Using CloudFormation to define and manage resources programmatically.
- **AWS Networking** 🌐: Implementing secure networking with VPCs, subnets, and routing.
- **Security Best Practices** 🔒: Configuring IAM roles and security groups to protect data and applications.

## 👤 About the Author
I'm a Computer Science student at the University of Florida with a strong interest in cloud engineering. This project is part of my journey to master building scalable, robust, and secure infrastructures on AWS. I’m focused on developing hands-on skills in cloud architecture and automation, setting the foundation for a future career in cloud technology. Feel free to connect if you’d like to discuss cloud projects or collaboration opportunities!
- **LinkedIn**: https://www.linkedin.com/in/matt-good/
- **Email**: mgoodman624@gmail.com
