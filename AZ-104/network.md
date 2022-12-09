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

## implement a Service Bus queue that guarantees first-in-first-out (FIFO) delivery of messages. 
- Enable sessions.
> Through the use of messaging sessions you can guarantee ordering of messages, that is first-infirst-out (FIFO) delivery of messages.

## Enable Floating IP.
> configure an Azure internal load balancer as a listener for the availability group.