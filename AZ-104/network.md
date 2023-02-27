## A virtual network can create two gateway
- VPN gateway: connectivity
  > site-to-site VPN connections  
    point-to-site VPN connections   
    vnet-to-vnet VPN connections 
- ExpressRoute gateway

## vpn gateway
> site-to-site need create gateway subnet
  
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
> NIC can not move to a new resource groupcan't move to a new resource group a NIC that is attached to a virtual machine.

## NSG apply to VM
> Destination with vm IP

## 302 Cannot just move a virtual machine between networks. 

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
- enables you to configure and track connection reachability, latency, and network topology changes. If there is an issue, it tells you why it occurred and how to fix it.
- monitors communication at a regular interval and informs you of reachability, latency, and network topology changes between the VM and the endpoint

## implement a Service Bus queue that guarantees first-in-first-out (FIFO) delivery of messages. 
- Enable sessions.
> Through the use of messaging sessions you can guarantee ordering of messages, that is first-infirst-out (FIFO) delivery of messages.

## Enable Floating IP.
> configure an Azure internal load balancer as a listener for the availability group.

## (Name server)NS record for the zone
> delegate a subdomain named research.adatum.com to a different DNS server 


## load balancer （351）
- Basic tier  : A load balancer is restricted to a single availability set, virtual machine scale set, or a single machine.
- Standard tier : can span any virtual machine in a single virtual network, including blends of scale sets, availability sets, and machines.

## Azure application gateway
> a web traffic load balancer that enables you to manage traffic to your web applications. it provides features such as session affinity,SSL offload，and cooki-based affinity to enable efficient distribution of traffic to multiple servers. 
> A useful tool for managing and optimizing the traffic to your web applications in Azure.
> Verify that you have a working virtual network with a valid subnet. Make sure that no virtual machines or cloud deployments are using the subnet. The application gateway must be by itself in a virtual network subnet.

## When creating Azure Bastion, it requires some configuration,
> 1. Subnet name must be "AzureBastionSubnet".
> 2. Subnet size must be /26 or larger.
> 3. For host scaling /26 is recommended

## a network interface
> A network interface (NIC) is the interconnection between a virtual machine and a virtual network. A virtual machine must have at least one NIC. A virtual machine can have more than one NIC, depending on the size of the VM you create. To learn about the number of NICs each virtual machine size supports, see VM sizes.  
You can create a VM with multiple NICs, and add or remove NICs through the lifecycle of a VM. Multiple NICs allow a VM to connect to different subnets.  
> - Each NIC attached to a VM must exist in the same location and subscription as the VM. Each NIC must be connected to a VNet that exists in the same Azure location and subscription as the NIC. You can change the subnet a VM is connected to after it's created. You can't change the virtual network. Each NIC attached to a VM is assigned a MAC address that doesn't change until the VM is deleted.

## A standard load balancer 
- is required for the HA ports.
- Two backend pools are needed as there are two services with different IP addresses.
- Floating IP rule is used where backend ports are reused.
- sku https://learn.microsoft.com/en-us/azure/load-balancer/skus#skus

## A resource can only be created in a virtual network that exists in the same region and subscription as the resource.

## 257：Azure Backup will be able to back up the unmanaged hard disks of the virtual machines in the storage account  
- never unless allow below
> Allow trusted Microsoft services to access this storage account as an exception to enable Azure Backup service to access the network restricted storage account.


## an application gateway that uses the WAF tier
> Azure Web Application Firewall (WAF) on Azure Application Gateway provides centralized protection of your web applications from common exloits and vulnerabilities.

## Resource on which to enable diagnostics:
> basic internal load balancer named |ILB1.

## Azure Traffic Manager 
> is a DNS-based traffic load balancer. This service allows you to distribute traffic to your public facing applications across the global Azure regions. Traffic Manager also provides your public endpoints with high availability and quick responsiveness.

##  point to site need the certificate
> Each client computer that connects to a VNet using Point-to-Site must have a client certificate
installed.
> You generate a client certificate from the self-signed root certificate, and then export and install the client certificate. If the client certificate is not installed, authentication fails.

## 335 Azure DNS supports importing and exporting zone files by using the Azure command-line interface (CLI). Zone file import is not currently supported via Azure PowerShell or the Azure portal.

## 336 direct all the Remote Desktop Protocol (RDP) connections to VM3 only.
> an inbound NAT rule

### 352 Private DNS zones you can link to VNET1 and the DNS zones to which VM1 can automatically register.
> the private zones only  
  >> To resolve the records of a private DNS zone from your virtual network, you must link the virtual network with the zone. Linked virtual networks have full access and can resolve all DNS records published in the private zone. You can also enable autoregistration on a virtual network link. When you enable autoregistration on a virtual network link, the DNS records for the virtual machines in that virtual network are registered in the private zone. When autoregistration gets enabled, Azure DNS will update the zone record whenever a virtual machine gets created, changes its' IP address, or gets deleted.

### public zone
> You can configure Azure DNS to resolve host names in your public domain. For example, if you purchased the contoso.xyz domain name from a domain name registrar, you can configure Azure DNS to host the contoso.xyz domain and resolve www.contoso.xyz to the IP address of your web server or web app.

### 372 ensure that VWebApp1 can be accessed only from computers on your on-premises network. 
> - B1 (Basic) would minimize cost compared P1v2 (premium) and $1 (standard).
> - Cross Origin Resource Sharing (CORS)
  >> Once you set the CORS rules for the service, then a properly authenticated request made against the service from a different domain will be evaluated to determine whether it is allowed according to the rules you have specified.

### 376 Ensure that all Internet-bound traffic from VNet1 is routed through the specific site : for example New York office.
> 1. Set-AzureRmVirtualNetworkGatewayDefaultSite
  >> The Set-AzureRmVirtualNetworkGatewayDefaultSite cmdlet assigns a forced tunneling default site to a virtual network gateway.
> 2. set traffic selector to vnet1 ip 

###  upload certificates to WebApp1 for HTTPS to access WebApp1.
> 1. Certificate format for HTTPS access:
  >> A PFX file contains the public key file (SSL Certificate) and its unique private key file. This is required for HTTPS access. The web app will distribute the public key (in a CER file) to clients that connect to the web app.
> 2. Certificate format for external service access:
  >> The CER file is an SSL Certificate which has the public key of the external service. The external service will have the private key associated with the public key contained in the CER file.

### 387 deploy a standard, Internet-facing load balancer named slb1.need to configure slb1 to allow connectivity to VM1. 
> 1. Before you create a backend pool on slb1, you must:
  >> Create and assign an NSG to VM1
> 2. Before you can connect to VM1 from slb1, you must:
  >> Create and configure an NSG

### #89 resolve name: www.contoso.com to the IP: 131.107.1.10 IP
> 1. create an Azure DNS zone named contoso.com, and then you add an A record to the zone for a host named www that has an IP address of 131.107.1.10.
> 2. Delegate the domain

### 406 The virtual machine you attach a network interface to and the virtual network you connect it to must exist in the same location, here West US, also referred to as a region.

### 409 add the network interface to must also exist in the same location and subscription as the network interface.
> A virtual network is required when you create a NIC. Select the virtual network for the network interface.  You can only assign a network interface to a virtual network that exists in the same subscription and location as the network interface. Once a network interface is created, you cannot change the virtual network it is assigned to. The virtual machine you add the network interface to must also exist in the same location and subscription as the network interface.

## Meaning that VM <--> VNET <---> NIC. All the three resources MUST be in the same location 

## 413 NSGs deny all inbound traffic except from virtual network or load balancers.

## 434  The virtual machines can successfully connect to the DNS server that has an IP address of 192.168.10.15 and the DNS server that has an IP address of 193.77.134.10.
> 1. VM1 uses the VNET configured DNS 193.77.134.10
> 2. VM2 uses the NIC configured DNS 192.168.10.15
> 3. VM3 uses the NIC configured DNS 192.168.10.15

## 436 delegate a subdomain named research.adatum.com to a different DNS server in Azure.
> You need to create a name server (NS) record for the zone.

## 444 Azure supports the following types of peering:
> 1. Virtual network peering: Connect virtual networks within the same Azure region.
> 2. Global virtual network peering: Connecting virtual networks across Azure regions.

## 453 perform a reverse DNS lookup for 10.0.0.4(vm1) from VM2.
> (FQDN will be return): vm1.azure.com

### 396 ensure that the administrators can access the Azure portal only from your onpremises network.
> the multi-factor authentication service settings.
> Once 'Additional cloud-based MFA settings' is clicked it takes you to the 'multi-factor authentication' Service settings page which gives you the option to configure trusted IP location to prevent MFA prompts for said location.

### 54 default inbound and outbound NSG rules which does not include port 3389.


- endpoints
> Endpoints are enabled on subnets configured in Azure virtual networks. Endpoints can't be used for traffic from your premises to Azure services. For more information, see Secure Azure service access from on-premises 

-  IKEv1
> tunneling protocol You plan to deploy route-based Site-to-Site VPN connections between several on-premises locations and an Azure virtual network. 

- NSG(network security groups) -> associated to NIC
> NSG's can be applied to NIC's or Subnets.

- NIC(network interface) -> associated to Vnet (virtual network)
- ALSO NIC： An Azure Virtual Machine (VM) has one or more network interfaces (NIC) attached to it. Any NIC can have one or more static or dynamic public and private IP addresses assigned to it.
> 5 VM so 5 NIC Cards .we have public and private ip address set to them .however they needs same inbound and outbound rule so create NSG and attach to NIC and this req can be fulfilled 5 NIC hence 5 is right ans

- DNS server # 511 order of DNS that server apply 
> Server3 --> NIC3 ---> VNET2 --> DNS settings on Virtual network "10.10.0.4"

- DNS auto register
> 1.  Public Ips wont auto register DNS,only manualy add public ips in public dns
> 2. Only private AZ DNS Zones can use auto registration

- 3389 used TCP
- VNet peering the only consideration is that the VNets do not overlap. VNET1 and VNETA do not overlap.
- No To create a VNet to VNet VPN you need to have a special Gateway Subnet. Here, the VNet has no sufficient address space to create a Gateway Subnet and thus to establish a VNet to VNet VPN connection.
- enable Floating IP ： configure an Azure internal load balancer as a listener for the availability group.

- load balancing
> 1. Frontend IP address
> 2. Backend pool
> 3. Inbound load-balancing rules
> 4. Health probe

- Set-AzureStaticVNetIP  
> Specify a static internal IP for a previously created VM If you want to set a static IP address for a VM that you previously created, you can do so by using the following cmdlets. If you already set an IP address for the VM and you want to change it to a different IP address, you'll need to remove the existing static IP address before running these cmdlets. See the instructions below to remove a static IP.


- You can set DNS servers per VM or cloud service to override the default network settings.
> NIC override the DNS server dns ip

- #6 view the average round-trip time (RTT) of the packets from VM1 to VM2.
> The connection monitor : capability monitors communication at a regular interval and informs you of reachability, latency, and network topology changes between the VM and the endpoint Incorrect Answers:

- The IP flow verify : capability enables you to specify a source and destination IPv4 address, port, protocol (TCP or UDP), and traffic direction (inbound or outbound). IP flow verify then tests the communication and informs you if the connection succeeds or fails. If the connection fails, IP flow verify tells you which security rule allowed or denied the communication, so that you can
resolve the problem.

- #19 A Site-to-Site VPN gateway connection can be used to connect your on-premises network to an Azure virtual network over an IPsec/IKE (IKEv1 or IKEv2) VPN tunnel.  This type of connection requires a VPN device, a VPN gateway, located on-premises that has an externally facing public IP address assigned to it.

- #19 Application Proxy is a feature of Azure AD that enables users to access on-premises web applications from a remote client.

- #17 A VPN gateway is used when creating a VPN connection to your on-premises network.
> Delete Existing GW and create New route-based GW
> When you create the virtual network gateway for a VPN gateway configuration, you must specify a VPN type. The VPN type that you choose depends on the connection topology that you want to create. For example, a P2S connection requires a RouteBased VPN type. A VPN type can also depend on the hardware that you're using. S2S configurations require a VPN device. Some VPN devices only support a certain VPN type
> PolicyBased VPNs can only be used on the Basic gateway SKU. This VPN type is not compatible with other gateway SKUs.

- #20 ensure that NGINX is available on all the virtual machines after they are deployed.
> 1. Azure Custom Script Extension
> 2. Desired State Configuration (DSC) extension

- #44 
> could endpoint: A sync group must contain one cloud endpoint 
> server endpoint: one or more server endpoint can be added to sync group

- # 54  default NSG rules, which denies any port open for inbound rules

- There is no overlap between the VNets:
> VNet1: 10.0.0.0/16 - CIDR IP Range 10.0.0.0 - 10.0.255.255
> VNet2: 10.10.0.0/24 - CIDR IP Range 10.10.0.0 - 10.0.0.255