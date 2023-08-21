# NAT, routes, Internet Gateway
​
Answer the following questions
​
1. What do you think the purpose of an internet gateway is? What would we not be able to do without one?

The purpose of the internet gateway is to allow traffic to flow in and out of the local network. With it, the local network or VPC would not be able to communicate with the outer world.

2. Thinking back to a previous session, where do you think you might be using a NAT gateway right now?

NAT gateways connect private subnets with the outer world usually for the purpose of updating devices in the subnets.

3. What IP addresses will be matched by the CIDR block of `0.0.0.0/0`?
   - for bonus points, explain why?

All IP addresses in the IPv4 will be matched by this CIDR block. 

4. In your own words, what is the difference between a NAT gateway and an Internet Gateway? When would you want one over the other?

The different between a NAT gateway and internet gateway is that the NAT gateway sits inside the public subnet and allows the private subnet to connect to the external internet. It protects the private subnets IP from the outer world. The internet gateway allows access to the public subnet. When connecting the private subnet you will use the NAT gateway, when connecting the public subnet you will use the internet gateway. 