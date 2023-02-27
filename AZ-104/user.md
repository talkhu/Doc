## to verify whether they still require the Security Administrator role.
- From Azure AD Privileged Identity Management, create an access review.

## enable two-step verification for Azure users.to enable two-step verification for Azure users.
- Create an Azure AD conditional access policy.

## Licensing Issue
> You attempt to assign a license in Azure to several users and receive the following error
> message: "Licenses not assigned. License agreement failed for one user."





## 254 & 343
> 1. You can't manually add or remove a member of a dynamic group.  Dynamic rules are based on a written logic and not manually managed by users.

> 2. Azure AD registered devices utilize an account managed by the end user, this account is either a Microsoft account or another locally managed credential.

> 3. Assigned groups - Manually add users or devices into a static group. Azure AD joined or hybrid Azure AD joined devices utilize an organizational account in Azure AD

## # 120  about Office 365 license assigned ,group3 = Office 365 license assigned and no rule 
 (Assigned = manual assignment/ Dynamic = Automatic assignment based on the membership rule)
Group3 as the membership type of "Assigned" so Users must be manually assigned to the group.

## The goal of Azure AD registered 
- also known as Workplace joined - devices is to provide your users with support for bring your own device (BYOD) or mobile device scenarios. In these scenarios, a user can access your organization’s resources using a personal device.

## Azure AD joined devices 
- are signed in to using an organizational Azure AD account. Access to resources can be controlled based on Azure AD account and Conditional Access policies applied to the device.



## invite the external partner to sign in to the Azure AD tenant.
> From the Users blade, modify the External collaboration settings.

## 312 assign a policy to the tenant root management group.
> - Assign the Owner role for the Azure subscription to User1, and then instruct User1 to configure access management for Azure resources.   
> - Each directory is given a single top-level management group called the "Root" managementgroup. This root management group is built into the hierarchy to have all management groups and subscriptions fold up to it. This root management group allows for global policies and Azure role assignments to be applied at the directory level. The Azure AD Global Administrator needs to elevate themselves to the User Access Administrator role of this root group initially. After elevating access, the administrator can assign any Azure role to other directory users or groups to manage the hierarchy. As administrator, you can assign your own account as owner of the root management group.

## 315 enable traffic analytics
> Your account must have any one of the following Azure roles at the subscription scope: owner, contributor, reader, or network contributor.

## 316 deploy virtual machines and manage virtual networks.
- Contributor not virtual machine contributor
> Virtual Machine Contributor don't have permission to manage networks.  

## 344 modify the JobTitle
> You must use Windows Server Active Directory to update the identity, contact info, or job info for users whose source of authority is Windows Server Active Directory.

### 350  Your on-premises network contains an Active Directory domain named adatum.com that is
synced to Azure Active Directory (Azure AD). Password writeback is disabled.
>  User must change password at next logon.

### 357 Require MFA for admins is a baseline policy that requires MFA for the following directory roles:
- Global administrator
- SharePoint administrator
- Exchange administrator
- Conditional access administrator
- Security administrator

### 358 enable two-step verification for Azure users.
> Create a single sign-in risk policy in Azure AD Identity Protection.

### 359 ensure that a service running on VM1 can manage the resources in RG1 by using the identity of VM1.
> From the Azure portal, modify the value of the Managed Service Identity option for VM1.
  >>  managed identity from Azure Active Directory allows your app to easily access other AADprotected resources such as Azure Key Vault. The identity is managed by the Azure platform and
does not require you to provision or rotate any secrets.
User assigned managed identities can be used on Virtual Machines and Virtual Machine Scale
Sets.

### 361 secure the members of the Lab Creator role. The solution must ensure that the lab creators request access when they create labs.
> From Azure AD Privileged Identity Management, edit the role settings for Lab Creator.  
>> As a Privileged Role Administrator you can: Enable approval for specific roles Specify approver users and/or groups to approve requests View request and approval history for all privileged roles

### 364 ensure that the users can use the email applications on their mobile device.
> Create an app password.

### 362 receive an email notification when any user activates an administrative role.(Basic Azure Active Directory (Azure AD))
> Purchase Azure AD Premium P2 and configure Azure AD Privileged Identity Management.
  >> Explanation:
When key events occur in Azure AD Privileged Identity Management (PIM), email notifications
are sent.
For example, PIM sends emails for the following events:  
When a privileged role activation is pending approval  
When a privileged role activation request is completed  
When a privileged role is activated  
When a privileged role is assigned  
When Azure AD PIM is enabled

### 365 enable MFA for the users in Tenant2. The solution must maintain MFA for Tenant1.
> Create and link a subscription to Tenant2.

### 370
> - App1: A service Bus queue  
> In Queues each message is processed by a single consumer.  
> - App2: A Service Bus topic  
> In contrast to queues, in which each message is processed by a single consumer, topics and subscriptions provide a one-to-many form of communication, in a publish/subscribe pattern.

### 414 provide users with the ability to bypass MFA for 10 days on devices to which they have successfully signed in by using MFA.
> From the multi-factor authentication page, configure the service settings.
  >> On the Service Settings page, manage remember multi-factor authentication, select the Allow users to remember multi-factor authentication on devices they trust option.  6. Set the number of days to allow trusted devices to bypass two-step verification. The default is 14 days.

### 415 Plan to share a cloud resource to the All Users group.
> Modify the Directory-wide Groups settings.

### 417 ensure that you can enable Azure Multi-Factor Authentication (MFA) for all users.
> requires a user account in Azure AD. not microsoft user

### 426 Each client computer that connects to a VNet using Point-to-Site must have a client certificate installed.  You generate a client certificate from the self-signed root certificate, and then export and install the client certificate. (need install) If the client certificate is not installed, authentication fails.

### 442  who will receive an email notification when Alert is triggered.
> Email will only be sent to Azure AD user members of the Monitoring Reader role. Email will not be sent to Azure AD groups or service principals.

### 543 upload files by using the Azure portal. The solution must use the principle of least privilege.
> Reader(it's a manager role)
> Storage Blob Data Contributor

---
- select the User must change password at next logon account option
for User.
1. He may be prompted to change, but it will not work unless Password write back is enabled..Hence he will not be allowed to sign in

- Resource Policy Contributor for subscription
> 1. create initiative definitions. 
> 2. User can assign initiatives. 

- dministrative-units
> three offices and an Azure subscription that contains an Azure Active Directory (Azure AD) tenant.

- Administrator accounts 
> are special accounts with elevated permissions. To secure them, the following restrictions apply to changing passwords of administrators: On-premises enterprise administrators or domain administrators cannot reset their password through Self-service password reset (SSPR). They can only change their password in their onpremises environment. Thus, we recommend not syncing on-prem AD admin accounts to Azure AD. An administrator cannot use secret Questions & Answers as a method to reset password.

- "Bulk Create" is for new Azure AD Users.
For Guests:
- Use "Bulk invite users" to prepare a comma-separated value (.csv) file with the user information and invitation preferences
- Upload the .csv file to Azure AD
- Verify the users were added to the directory

- #9 need be invited to new tenant: When you make a new tenant the global admin who created the new tenant is then added as a global admin for the new tenant (as an external user). BUT any other global admin in the old
tenant are not automatically added to the new tenant unless you manually invite them later.

- #10 Only a global administrator can add users to this tenant.

- #12 OAuth 2.0 protocol(authorization endpoint) is used when it comes to kubenentes
- #13 You can set expiration policy only for Office 365 groups in Azure Active Directory (Azure AD).

- #22 Assign a role to a user
> From the Directory role blade, modify the directory role

### Device settings from the Devices blade.
> When you connect a Windows device with Azure AD using an Azure AD join, Azure AD adds the
following security principles to the local administrators group on the device:
>>- The Azure AD global administrator role
>>- The Azure AD device administrator role
>>- The user performing the Azure AD join