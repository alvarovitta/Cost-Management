# Assessing your Azure Migration Cost
Use the information and procedure described in this section to assess and plan your workloads in Azure.
<br />
<br />

Consider the costs associated with migrating applications or systems to Azure. Use the Microsoft tool: *Azure Migrate* to assess the scale of workload migration and estimate the costs for running on-premises machines in Azure.

Azure Migrate calculates an estimate of costs associated with the post-migration compute and storage environment. Estimates are calculated based on sizing requirements for a virtual machine (VM) and its disks.
<br />
<br />

Azure Migrate calculates:  
- **Total monthly compute cost of all machines**: VM cost calculation is based on the recommended VM size. Total cost is an aggregate of cost across all machines. Calculation variables include: operating system, software assurance, reserved instances, VM uptime, location, and currency settings. 

- **Total monthly storage costs of all machines**:  Costs are displayed in the currency specified in the assessment settings. *Note*: The calculation doesn't include offers specified in the assessment settings. 

The figure below illustrates an example of a completed assessment. The estimate includes monthly costs for compute and storage for each machine.
<br/>
<br/>

![assessment](https://github.com/alvarovitta/Cost-Management/blob/master/Images/assessment-vm-cost.png)
<br/>
<br/>

## Guidance
Use the following guidance in assessing and planning your workloads to Azure.

- Understand [How Azure Migrate Works](https://docs.microsoft.com/en-us/azure/migrate/migrate-overview#how-does-azure-migrate-work)

- Before running an assessment, [group machines using machine dependency mapping](https://docs.microsoft.com/en-us/azure/migrate/how-to-create-group-machine-dependencies#prepare-machines-for-dependency-mapping). Grouping VMs helps you to visualize the dependencies of your machines and to effectively plan your migration to Azure.  

  Grouping VMs will:
   - ensure that nothing is left behind  
   - discover all the interdependent systems that need to migrate together  
   - identify whether a running system is still serving users and/or is a candidate for decommissioning instead of migration.

- When you use Azure Migrate to conduct an assessment of your VMs, keep machines with interdependencies within the same project and assessment. If for example, you are using vCenter Server, ensure that dependent machines are in the same folder, datacenter, or cluster. 

- Customize the default [assessment properties](https://docs.microsoft.com/en-us/azure/migrate/how-to-modify-assessment#edit-assessment-properties) in Azure migrate according to your requirements
<br/>
<br/>

## Preparation
Perform the following activities before you begin the assessment procedure tasks: 

  - Review and understand the [prerequisites](https://docs.microsoft.com/en-us/azure/migrate/how-to-scale-assessment#prerequisites)
  
  - Review the [port requirements](https://docs.microsoft.com/en-us/azure/migrate/migrate-overview#what-are-the-port-requirements) for Azure Migrate
  - [Plan your migration projects and discoveries](https://docs.microsoft.com/en-us/azure/migrate/how-to-scale-assessment#plan-your-migration-projects-and-discoveries)
<br/>
<br/>

## Procedure 
Perform the procedure as noted in the link: [how to assess your on-premises VMware VMs for migration to Azure](https://docs.microsoft.com/en-us/azure/migrate/tutorial-assessment-vmware)
<br/>
<br/>

## Next steps
[Designing your Azure Subscription for Cost Management](3.2-Designing-your-Azure-subscription-for-cost-management.md)

