## Integrate a NAT gateway with a public load balancer using Terraform

### In this tutorial, we will integrate a NAT gateway with a public load balancer.

#### By default, an Azure Standard Load Balancer is secure. Outbound connectivity is explicitly defined by enabling outbound SNAT (Source Network Address Translation). SNAT is enabled in a load-balancing rule or outbound rules.

#### The NAT gateway integration replaces the need for outbound rules for backend pool outbound SNAT.