## Integrate a NAT gateway with a public load balancer using Terraform

### In this tutorial, we will integrate a NAT gateway with a public load balancer.

#### By default, an Azure Standard Load Balancer is secure. Outbound connectivity is explicitly defined by enabling outbound SNAT (Source Network Address Translation). SNAT is enabled in a load-balancing rule or outbound rules.

#### The NAT gateway integration replaces the need for outbound rules for backend pool outbound SNAT.
#### Use Bastion to access a VM and in Powershell type: curl ifconfig.me - this command should show the same IP-address as the Public-IP of the NAT-GW.
#### Access your FrontendIP of your loadbalancer in the browser. It should display either "Hello World from non-prod-vm2" or "Hello World from non-prod-vm1".

#### This shows us the loadbalancer is working for inbound connections and the Nat-GW is working for outbound connections integrated within the same subnet as the loadbalancer.

##### reference link: https://learn.microsoft.com/en-us/azure/nat-gateway/tutorial-nat-gateway-load-balancer-public-portal