# multI-resource_begginer_Terraformlab_Azure
Deploy a Web-Ready Azure Environment with Terraform

# What you'll Build
• 	Resource Group
• 	Virtual Network + Subnet
• 	Network Security Group
• 	Azure VM (Ubuntu)
• 	Public IP + NIC
• 	Storage Account
• 	Output IP for SSH access

# Folder Structure
azure-terraform-lab/
├── main.tf
├── variables.tf
├── outputs.tf
├── ssh-key/
│   ├── id_rsa
│   └── id_rsa.pub
└── README.md

## Deployment Steps
# Generate SSH Keys:
mkdir ssh-key && ssh-keygen -t rsa -b 2048 -f ssh-key/id_rsa
# Authenticate:
az login
# Initialize and apply:
terraform init
terraform apply

# Learning Outcomes
• 	Understand Terraform modules and resource dependencies.
• 	Practice provisioning compute, networking, and security.
• 	Learn how to use outputs and SSH into VMs.
