VPC created with name 3tier-vpc, CIDR 10.99.0.0./16 choosen
6 subnets:2 public + 4 private have been created by using 2 AZ:
-DMZ1-public (us-west-1a)
-DMZ2-public (us-west-1b)
-AppLayer1-private (us-west-1a)
-AppLayer2-private (us-west-1b)
-DBLayer1-private (us-west-1a)
-DBLayer2-private (us-west-1b)
Internet Gateway created under name 3tier-igw and attached to VPC
NAT Gtaeway has been created by using DMZ2-public subnet and elastic IP allocated
I have created 2 Route Table
-public for- DMZ1-public and DMZ2-public, Route (IGW)+Subnet assosiaction done 
-private for - rest 4 subnets, Route (NAT Gateway)+Subnet assosiaction done
3 NACLs created: 1)DMZNacl; 2)AppLayerNacl; 3)DBLayerNacl
Inbound + Outbound rules for NACLs done