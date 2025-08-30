VPC	 10.0.0.0/16	          ------> Main VPC
Public Subnet	10.0.1.0/24	  ------> Internet accessible
Private Subnet 10.0.2.0/24	------> No Internet by default
IGW	                        ------> Attached to VPC	Routes traffic out
Route Table	PublicRouteTable------>	Routes 0.0.0.0/0 to IGW
EC2 Instance	              ------> In PublicSubnet	Public IP, SSH enabled
