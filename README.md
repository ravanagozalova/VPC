VPC created under name VPC_diagram1 with IP 10.0.0.0/16
Internet gateway created under name IGW_diagram and attached to VPC that I created
4 subnets - 2 public and 2 private should be created
1st Subnet created as VPC_subnet1 with 1AZ, IPv4 CIDR block choosen - 192.168.0.0/26
2 AZ us-east-1a and us-east-1b were choosen for public subnets and for private subnets
    - subnet-1-public (10.0.1.0/24)
    - subnet-2-public (10.0.2.0/24)
    - subnet-1-private(10.0.3.0/24)
    - subnet-2-private(10.0.4.0/24)
  2 Route Tables should be created : 1 public and 1 private
    - 1 RT-public - edit RT- add routes -0.0.0.0/0 and IGW choosen (route to the internet activated) and subnet assosiations done for public RT+public subnets
    - 2 RT-private - edit RT -add routes - 0.0.0.0/0 and IGW choosen (route to the internet activated) and subnet assosiations done for private RT+private subnets
  NACL-public and NACL-private were created, Inbound and Outbound rules set up.Subnet assosiaction done between them.
2 Security Groups -public and private are created and inbound + outboud rules added.
  
