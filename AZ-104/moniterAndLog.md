# NetWork Mointor
## Metrics in Application Gateway
> Application Gateway currently has seven metrics to view performance counters. Metrics are a
feature for certain Azure resources where you can view performance counters in the portal. For
Application Gateway, the following metrics are available:
>> 1. Total Requests
>> 2. Failed Requests
>> 3. Current Connections
>> 4. Healthy Host Count
>> 5. Response Status
>> 6. Throughput
>> 7. Unhealthy Host count  
>> You can filter on a per backend pool basis to show healthy/unhealthy hosts in a specific backend pool

## create an alert in Azure when more than two error events are logged to the System event log on VM1 within an hour.
> create an Azure Log Analytics workspace and configure the data settings. You add the Microsoft Monitoring Agent VM extension to VM1. You create an alert in Azure Monitor and specify the Log Analytics workspace as the source.

## AZ monitor
- create a alert from Azure Log Analytics as resource  
> Alerts in Azure Monitor can identify important information in your Log Analytics repository. They are created by alert rules that automatically run log searches at regular intervals, and if results of the log search match particular criteria, then an alert record is created and it can be configured to perform an automated response.

## view the error from a table named Event from Azure log Analytics workspace.
> Event | search "error"

## view the error events from a table named Event.
> search in (Event) "error"

## 401 creating an alert rule in Azure Monitor to notify an administrator when an error is logged in the System event log of VM. 
> virtual machine extension
  >> Azure Monitor can collect data directly from your Azure virtual machines into a Log Analytics workspace for detailed analysis and correlation. Installing the Log Analytics VM extension for Windows and Linux allows Azure Monitor to collect data from your Azure VMs.

## 404 When you want to delete the resource, you first need to remove the lock.

## 446 ：VM2 is backed up to RSV1.  You need to back up VM2 to RSV2.
> From the VM2 blade, click Disaster recovery, click Replication settings, and then select RSV2 as the Recovery Services vault

## 442 Email will only be sent to Azure AD user members of the Monitoring Reader role. Email will not be sent to Azure AD groups or service principals.

- Azure Monitor 
> Metrics in Azure Monitor are stored in a time-series database which is optimized for analyzing time-stamped data. This makes metrics particularly suited for alerting and fast detection of issues.
-  inspect all the network traffic
>  use the Packet Capture

- create an alert in Azure : when more than two error events are logged to the System event log on VM1 within an hour.
> 1. You create an Azure Log Analytics workspace and configure the Agent configuration settings. You install the Microsoft Monitoring Agent on VM1. You create an alert in Azure Monitor and specify the Log Analytics workspace as the source.
> 2. Alerts in Azure Monitor can identify important information in your Log Analytics repository. They are created by alert rules that automatically run log searches at regular intervals, and if results of the log search match particular criteria, then an alert record is created and it can be configured to perform an automated response.                   The Log Analytics agent collects monitoring data from the guest operating system and workloads of virtual machines in Azure, other cloud providers, and on-premises. It collects data into a Log Analytics workspace.

- Live metrics stream includes : such information as the number of incoming requests, the duration of those requests, and any failures that occur. You can also inspect critical performance metrics such as processor and memory.

- Retention is available only if you use General purpose v2 Storage accounts (GPv2).

- Azure Monitor -> Azure Monitor?a Log Analytics workspace a resource,

- monitor the metrics and the logs of VM1.
> Linux Diagnostic Extension (LAD) 3.0