# TAG
##### 348 Tags applied to the resource group are not inherited by the resources in that resource group.
  
#### 458 associate each VM with its respective department.
> Assign tags to the virtual machines.

# maintain
#### 99 years
> backup With the latest update to Azure Backup, customers can retain their data for up to 99 years in
Azure.

#### 30 days: once backup default to 30 days
> default policy. This backs up the VM once a day at the time specified, and retains backups in the vault for 30 days.

#### 345 Azure backup only for VM
> 1. Azure Backup policies can only back up an Azure VM, SQL in an Azure VM or File Share. As such the answer to the first part should be Share1 only.

> 2. To create a vault to protect virtual machines, the vault must be in the same region as the virtual machines.

#### Use Azure Site Recovery to migrate the virtual machines to Azure.
> - Maximum Operating system disk size for a generation VM is 2,048 GB(2T)
> - Max data disk size is 4,095 GB(4T)
> - Bitlocker is not supported. BitLocker must be disabled before you enable replication


#### Fraud alert
> Configure the fraud alert feature so that your users can report fraudulent attempts to access their
resources. Users can report fraud attempts by using the mobile app or through their phone.
Configuration options include:
Block user when fraud is reported: If a user reports fraud, their account is blocked for 90 days or
until an administrator unblocks their account. An administrator can review sign-ins by using the
sign-in report, and take appropriate action to prevent future fraud. An administrator can then
unblock the user's account.

#### Connection Troubleshoot
> With the addition of Connection Troubleshoot, Network Watcher will see an incremental increase
in its capabilities and ways for you to utilize it in your day to day operations. You can now, for
example, check connectivity between source (VM) and destination (/M, URI, FQDN, IP Address).

#### VMZ2 is protected by RSV1. You need to use RSV2 to protect VM2.
> first: From the RSV1 blade, click Backup items and stop the VM2 backup. 

#### DevTest Labs User role only lets you connect, start, restart, and shutdown virtual machines in your Azure DevTest Labs.

#### slots to the Testing in production blade
> Besides swapping, deployment slots offer another killer feature: testing in production. Just like the
name suggests, using this, you can actually test in production. This means that you can route a
specific percentage of user traffic to one or more of your deployment slots.
Example:

##### View template from deployment history from resource group

##### azcopy make 
> coppy a contaner to Azure
> with blob type

#### 248 add Share1(with file1.txt) as an endpoint for Sync1. One hour later, you add Share’ as an endpoint for Sync1. One hour later, you add Share2 as an endpoint for Sync.
> File1.txt from Share1 replicates to Share2.

#### 10 update domain how to count
- Only one update
domain is rebooted at a time.
> 14 VMs : update domains will have two VMs and six update domains will have one VM. Only one update domain is rebooted at a time. Therefore, a maximum of two VMs will be offline.
- update domain max is 20

#### 2 fault domain
> 14 VMs : The 14 VMs are shared across the 2 fault domains, so 7 VMs in each fault domain. A rack failure will affect one fault domain so 7 VMs will be offline.

#### 270 move the web app to another reource grup with different region is ok but cannot change an App Service plan's region.

#### identify underutilized virtual machines that can have their service tier changed to a less expensive offering.
> Advisor

#### export and import 
> The service only supports Export of Azure Blobs. Export of Azure files is not supported. Import is supported for Azure Blob storage and Azure File storage as well.

#### synchronize the files in the file share named data to an on-premises server 
> - Register Server1
> - Install the Azure File Sync agent on Server1
> - Create a sync group

#### 297 blob storage support all the type of storage

#### 305 To install kubectl locally, use the az aks install-cli command:

#### 309 recovery points,  daily + weekly + monthly
> note: count weely point, over 1 weeky will be 2. 

#### 317 Azure Import/Export service to copy files to a storage account.
- a dataset CSV file
- a driveset CSV file

> Modify the dataset.csv file in the root folder where the tool resides. Depending on whether you want to import a file or folder or both, add entries in the dataset.csv file Modify the driveset.csv file in the root folder where the tool resides.

#### 322 who is the local administrator
> Azure AD. Global administrators, here User2, in Azure AD and device owners are granted local administrator rights by default.

#### To create a vault to protect virtual machines, the vault must be in the same region as the virtual machines.

#### 354 You can add the virtual machine to a scale set in the same region, Zone, and resource group.

#### 365 You conduct the initial migration assessment and get a message that some virtual machines are conditionally ready for Azure.  You need to find the cause of this message.
> - The operating system is configured as Windows Server 2003 in vCenter Server.
> - The VMs are configured with the UEFI boot type.

#### 368 Configurations so Azure Migrate service can collect all of the available information.
> Configure the data collector level in VMware vCenter to level 3.
> Level3: Metrics for all counters, excluding minimum and maximum rollup values.

#### 390 Assessment and migration: In the Azure Migrate hub, you can assess and migrate:
> - Servers, databases, and web apps: Assess on-premises servers including web apps and SQL
> - Server instances and migrate them to Azure virtual machines or Azure VMware Solution
(AVS) (Preview).
> - Databases: Assess on-premises databases and migrate them to Azure SQL Database or to
> SQL Managed Instance.
> -  Web applications: Assess on-premises web applications and migrate them to Azure App
> Service.
> - Virtual desktops: Assess your on-premises virtual desktop infrastructure (VDI) and migrate it to
> Windows Virtual Desktop in Azure.
> - Data: Migrate large amounts of data to Azure quickly and cost-effectively using Azure Data Box
> products.

#### 368 make needed configurations so Azure Migrate service can collect all of the available information.
> Configure the data collector level in VMware vCenter to level 3.

#### 405 SQL Server in VM and NOT Azure SQL DB can be backed up using Service Vault. Hence it should be 2 (B) and not 3 as the answer.

#### 427 identify unattached disks that can be deleted.
> From Microsoft Azure Storage Explorer, view the Account Management properties

#### 429 add cloud endpoint and sharepoint point for sync group
> 1. A sync group must contain one cloud endpoint, which represents an Azure file share and one or more server endpoints.
> 2. data1 on server need registered to Sync

#### 443 file share and archive access tier
> 1. Premium file shares are hosted in a special purpose storage account kind, called a FileStorage account.
> 2. Use the Archive access tier in storageV2,storage,BlobStorage   

#### 503 Hyper-V server that hosts a VM, named VM1, which must be replicated to Azure. 
> 1. Hyper-V site
> 2. Azure Recovery Services Vault
> 3. Replication policy

### 103 : Remains available if a single data center in the region fails.
> Zone-redundant storage (ZRS) replicates your data synchronously across three storage clusters in a single region.

### 51 
Box 1: 4
> If you resize the Scale Set all the VMs get resized at once, thus 4 is the correct answer.

Box 2: 1
> Automatic OS updates update 20% of the VMs at once, with a minimum of 1 VM instance at a time. Also 20% of 4 = 0.8.

---
- Locks 
> are designed for any update or removal. In this case we want to move only, we are not deleting, and we are not changing anything in the resource.

- update domain: update domain max is 20
- fault domain: The number of fault domains for managed availability sets varies by region - either two or three
per region.

- Azure Backup supports :
> VM that are shutdown or offline.
> 64 bit windows(server from 2008) and linux(Debian 7.9+)

- BlockBlobStorage = Premium block blobs only available for Premium_LRS or Premium_ZRS.
- need to grant Group1 the Storage File Data SMB Share Elevated Contributor role for share1.  
> Enable Active Directory Domain Service (AD DS) authentication for storage1. 

- #3 If you try to deploy your own template in the portal, there are 3 available options - 
> 1. "Subscription", 
> 2. "Resource Group", 
> 3. "Location".

- #5 when an NSG is created, it automatically blocks TCP port 8080 between
the virtual networks.
>configure a custom policy definition, and then you assign the policy to the subscription.

- Azure Backup supports backup of 64-bit Windows server operating system from Windows Server 2008.

- Set-AzMarketplaceTerms - "Accept or reject terms for a given publisher id(Publisher), offer id(Product) and plan id(Name). Please use Get-AzMarketplaceTerms to get the agreement terms."

- #24 alert is set in Service Manager when the amount of available memory on VM1 is below 10 percent.
> The IT Service Management Connector (ITSMC): allows you to connect Azure and a supported IT Service Management (ITSM) product/service, such as the Microsoft System Center Service Manager.  With ITSMC, you can create work items in ITSM tool, based on your Azure alerts (metric alerts,Activity Log alerts and Log Analytics alerts).

- #26 Azure Import/Export service supports the following storage types:
> 1. Import supports Azure Blob storage Azure File storage 
> 2. Export supports Azure Blob storage

- #49 vault region:
> Storage Account must be in the same Region as the Recovery Services Vault.
>log analytics workspaces region : independindependent of the location and subscription where your Vaults exist.

- #53 route trough vm3
Given answer is correct.
> 1. address prefix- destination-> Vnet 1 (Address space of Vnet1)
> 2. Next Hop - VM1 ->Virtual Appliance (You can specify IP address of VM 1 when configuring next hop as virtual appliance)
> 3.Assignment - This route is to be followed by Gateway Subnet for the incoming traffic. You can associate routing table to the Subnet from Rout Table -> subnet ->Associate