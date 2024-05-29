Build the CloudFormation Template/Project of the following Architecture…



Resources:
VPC with 2 Su
Resources:
VPC with 2 Subnets (public) , IGW, Route-Table-with-Route (IGW), Subnet-Association-with-route-table
aws_vpc, aws_subnet, aws_internet_gateway, aws_route_table, aws_subnet, aws_route_table_association
1 SG for EC2 (22, 80 for all)
aws_security_group, aws_vpc_security_group_ingress_rule, aws_vpc_security_group_egress_rule
1 SG for ALB (80 for all)
aws_security_group, aws_vpc_security_group_ingress_rule, aws_vpc_security_group_egress_rule
1 SG for RDS (3306 for all)
aws_security_group, aws_vpc_security_group_ingress_rule, aws_vpc_security_group_egress_rule
1 ASG launch Template
aws_launch_configuration
1 AutoScal
ing Group with 2 EC2 Min
aws_autoscaling_group
ALB-Target-Group
aws_lb_target_group
ALB (2 Public Subnet)
aws_lb,, aws_lb_listener
S3 Bucket-Private [Override- Pass -var]
aws_s3_bucket
IAM Role (Assumed by EC2)
aws_iam_role
IAM Policy (S3:* FullAccess)
aws_iam_role_policy
RDS Subnet-Group (2 Subnets)aws_db_subnet_groupbnets (public), IGW, Route-Table-with-Route (IGW), Subnet-Association-with-route-table
aws_vpc, aws_subnet, aws_internet_gateway, aws_route_table, aws_subnet, aws_route_table_association
