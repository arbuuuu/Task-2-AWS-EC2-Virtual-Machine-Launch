Objective:

To understand how cloud virtual machines work by creating, configuring, and connecting to a cloud-based server instance using a free-tier AWS account.
This task helps in learning Infrastructure-as-a-Service (IaaS) — the foundation of cloud computing.


Create the VM Instance

Open the AWS Management Console → Search for EC2 → Click Launch Instance.

Name: any name (e.g., my-first-vm)

AMI (OS Image): Ubuntu Server 22.04 LTS (Free Tier eligible)

Instance Type: t2.micro (Free Tier eligible)

Key Pair: Create and download a new .pem key file for SSH access

Configure Network (Firewall)

In Network Settings, choose:

Auto-assign Public IP: Enable

Allow SSH traffic from anywhere (0.0.0.0/0)

Allow HTTP & HTTPS traffic (optional, for web apps)

Launch the Instance

Click Launch Instance.

Wait for the instance to show Running in the EC2 dashboard.

Note the Public IPv4 address (used to connect to the server).

Connect via SSH

Select your instance → Click Connect → Choose EC2 Instance Connect (browser-based SSH).

Run the following commands to verify connection:

uname -a
ls
whoami


Successful outputs confirm your VM is active and accessible.

Stop or Terminate the Instance

Go back to the EC2 Dashboard → Instances.

Choose Stop or Terminate when testing is complete to save free credits.

🧩 VM Configuration (Example Note)

OS: Ubuntu Server 22.04 LTS
Region: ap-south-1 (Mumbai)
Instance Type: t2.micro

💡 Outcome

By completing this task, I learned to:

Create and manage cloud servers using AWS EC2

Connect to a VM using SSH

Understand key IaaS concepts such as scalability, flexibility, and remote access
