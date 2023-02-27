#  Case Study 1 - Humongous Insurance
## 205,206,207,208,209,210,211,212

## Licensing Issue
- You attempt to assign a license in Azure to several users and receive the following error
 message: "Licenses not assigned. License agreement failed for one user."
 You verify that the Azure subscription has the available licenses.

  > From the Profile blade, modify the usage location.
  >> Explanation:
License cannot be assigned to a user without a usage location specified.

## Which blade should you instruct the finance department auditors to use?
- Invoices
> You can opt in and configure additional recipients to receive your Azure invoice in an email. This feature may not be available for certain subscriptions such as support offers, Enterprise Agreements, or Azure in Open.

---

# Case Study 2 - Contoso, Ltd

## 213,214,215,216,217



### 1. Change the Service administrator for an Azure subscription Sign in to Account Center as the Account administrator.
> From the Subscriptions blade, select the subscription, and then modify the Properties.

### 2. Move the blueprint files to Azure.
> Use Azure Storage Explorer to copy the files.

### 3. You need to implement a backup solution for App1 after the application is moved. What should you create first?
> create a Recovery Services vault

### 4. Number of virutal networks and subnets
- A SQL database
- A web front end
- A processing middle tier
> one virutal network
> three subnets
  >> one for web front  
  >> A processing middle tier  
  >> one for SQL database

### 5. blueprint file
- Blueprint 是一个存储操作方法的容器，这些操作在这个Blueprint 被注册到一个应用之后就可以被调用，
> need a blob type storge.


# Case Study 3 - Contoso, Ltd

## 219,220,221,222,223,224,225,226

### 1. Create a workflow to send an email message when the settings of VM4 are modified. event hub
> event hub

### 2. use conditional access policies that can then be targeted to groups of users, specific applications, or other conditions.
> dynamic groups and conditional access policies

### 3. Migrate the virtual machines hosted on Serverl and Server2 to Azure.
> 1. Create a Recovery Services vault
> 2. Install the Azure Site Recovery Provider
  >> Azure Site Recovery can be used to manage migration of on-premises machines to Azure.

### 4. Connect the New York office to VNet1 over the Internet by using an encrypted connection.
> 1. Create a virtual network gateway and a local network gateway. 
> 2. Configure a site-to-site VPN connection

### 5. create a role base reader role
- Get-AzureRmRoleDefinition
- ConvertTo-Json

# Case Study 4 - ADatum

## 225,226,227,228,229,230,231

### 1. A new web app named App1 that will access third-parties for credit card processing must be
deployed. 
- App Service Environment v1
> ASE1 and an App Service plan that uses the I1 pricing tier（ASEv1）
  >> app service 
> An App Service Environment is a Premium service plan option of Azure App Service that provides a fully isolated and dedicated environment for securely running Azure App Service apps at high scale.

### 2. Azure Application Gateway (internal)  AG1
AG1 must load balance incoming traffic in the following manner:
- htto://corporate.adatum.com/video/* will be load balanced across Pool11.
- http://corporate.adatum.com/images/* will be load balanced across Pool12.

> a URL path-based routing rule

### 3. AG2 must load balance incoming traffic in the following manner:
- htto:/Avww.adatum.com will be load balanced across Pool21.
- htto://fabrikam.com will be load balanced across Pool22.

> multi-site listeners

### 4. identify the appropriate sizes for the Azure virtual machines.
- From the Azure portal, create an Azure Migrate
assessment.
- From the Azure portal, download an OVA file.
- From VM1, run the Deploy OVF Template wizard.
- From VM1, connect to the collector virtual machine]
and run the Azure Migrate Collector.
- From the Azure portal, create an Azure Migrate
project.

### 5. A newly developed API must be implemented as an Azure function named App2. App2 will use a blob storage trigger. App2 must process new blobs immediately.
- This requires "Always On".
> The Standard pricing tier is the cheapest tier that supports Always On.

### 6. configure Azure ExpressRoute routing
- Routing from ADatum to Azure:
  > Use BGP to append the private AS numbers to the advertised prefixes.

- Routing from Microsoft Online Services to Adatum: 
  > Use BGP communities to configure BGP's Local Preference.

### IP address do not overlap

# Case Study 5 - Contoso, Ltd

#### 456 Create a blob container named container1 and a file share named share‘ that will use the Cool storage tier. 
> 1. storagev2,and blob storage for blob container(general storage not support cool tier)
> 2. storageV2 for file share with cool tier
  >> key world : cool storage tier 
     
