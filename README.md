# DevOps-Project
Full GitOps Pipeline on AWS with Terraform, Monitoring, Logging, and Secrets Management

# Terraform
```
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
```


```
                Internet
                    │
            Internet Gateway
                    │
         ┌──────────VPC──────────┐
         │                       │
   Public Subnets          Private Subnets
   ┌────────────┐         ┌──────────────┐
   │ Pub-1 AZ-a │         │ Priv-1 AZ-a │
   │ Pub-2 AZ-b │         │ Priv-2 AZ-b │
   │ Pub-3 AZ-c │         │ Priv-3 AZ-c │
   └────────────┘         └──────────────┘
         │                       │
         │ NAT Gateway           │
         └───────────────► Internet (via NAT)



```
