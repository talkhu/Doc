## A virtual network can create two gateway
- VPN gateway: connectivity
  > site-to-site VPN connections  
    point-to-site VPN connections   
    vnet-to-vnet VPN connections 
- ExpressRoute gateway
  
## type of DNS record 
> TXT record： App Services uses this record only at configuration time to verify that you
own the custom domain. 

## add contoso.com as a custom domain name to Azure AD.
>MX record： ensure that Azure can verify the domain name.

## UNC file share Path
> Azure Storage account + file.core.windows.net\ + data
> example: \\contosostorage.file.core.windows.net\data

## NIC (network interface)
> A NIC can only be attached to a single VM  
> just need one NSG : A NSG can be assigned to zero or more NICs or Subnets; since the rules need to be the same,only one NSG rule set is needed, which will be applied to each NIC.

## Azure DNS provides automatic registration of virtual machines from a single virtual network that's linked to a private zone as a registration virtual network. 

## Forward DNS resolution is supported across virtual networks that are linked to the private zone as resolution virtual networks.

## peering vnet
> 1. re peering need delete old disconnect peering rule,and recreate a new one.
> 2. The virtual networks you peer must have non-overlapping IP address spaces. 

## peering ping
> need peering vent each other for ping for example vm1 to vm2


## a virtual network link
>  1. After you create a private DNS zone in Azure, you'll need to link a virtual network to it. Once linked, VMs hosted in that virtual network can access the private DNS zone. Every private DNS zone has a collection of virtual network link child resources. Each one of these resources represents a connection to a virtual network. A virtual network can be linked to private DNS zone as a registration or as a resolution virtual network.
> 2. Registration virtual network : When creating a link between a private DNS zone and a virtual network. You have the option to enable autoregistration. With this setting enabled, the virtual network becomes a registration virtual network for the private DNS zone

## Collector communicates 
> - Collector communicates with Azure Migrate service over SSL 443.
> - The Collector must be able to communicate with the vCenter Server. By default, it connects to
vCenter on 443.

## Azure Network Watcher, you create a packet capture.
- example : Azure Network Watcher, you create a packet capture.
> Packet Capture can inspect 18000 seconds (5 hours) Network Status.

## Network Watcher packet capture
- allows you to create capture sessions to track traffic to and from
a virtual machine. Filters are provided for the capture session to ensure you capture only the traffic you want. Packet capture helps to diagnose network anomalies, both reactively, and proactively.

##  Network Watcher Connection Monitor 
- enables you to configure and track connection reachability,
latency, and network topology changes. If there is an issue, it tells you why it occurred and how to
fix it.

## implement a Service Bus queue that guarantees first-in-first-out (FIFO) delivery of messages. 
- Enable sessions.
> Through the use of messaging sessions you can guarantee ordering of messages, that is first-infirst-out (FIFO) delivery of messages.

## Enable Floating IP.
> configure an Azure internal load balancer as a listener for the availability group.

## (Name server)NS record for the zone
> delegate a subdomain named research.adatum.com to a different DNS server 


## load balancer 
- Basic tier  : A load balancer is restricted to a single availability set, virtual machine scale set, or a single machine.
- Standard tier : can span any virtual machine in a single virtual network, including blends of scale sets, availability sets, and machines.

## Azure application gateway
> a web traffic load balancer that enables you to manage traffic to your web applications. it provides features such as session affinity,SSL offload，and cooki-based affinity to enable efficient distribution of traffic to multiple servers. 
> A useful tool for managing and optimizing the traffic to your web applications in Azure.