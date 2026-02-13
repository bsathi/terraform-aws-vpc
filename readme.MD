# Terraform AWS VPC

This module creates the following resources.

## Resources Created
- VPC
- Internet Gateway (IGW)
- 2 Public subnets in us-east-1a and us-east-1b
- 2 Private subnets in us-east-1a and us-east-1b
- 2 Database subnets in us-east-1a and us-east-1b
- Public Route Table
- Private Route Table
- Database Route Table
- Elastic IP for NAT Gateway
- NAT Gateway in public subnet (us-east-1a)
- IGW route added to public route table
- NAT Gateway route added to private and database route tables
- Route table associations with subnets
- VPC peering to default VPC
- Public route table route to default VPC
- Default VPC main route table route to created VPC

## Inputs
- **vpc_cidr** (Required): CIDR block for the VPC
- **project_name** (Required): Project name used for tagging
