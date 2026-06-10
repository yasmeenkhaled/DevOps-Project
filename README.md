# DevOps-Project
Full GitOps Pipeline on AWS with Terraform, Monitoring, Logging, and Secrets Management

# Terraform
terraform/
│
├── provider.tf
├── variables.tf
├── outputs.tf
│
├── modules/
│   └── vpc/
│       ├── main.tf
│       ├── variables.tf
│       └── outputs.tf
│
└── environments/
    └── dev/
        ├── main.tf
        └── terraform.tfvars
