# Assessing your Azure Migration Cost

When assessing your on-premise migration to Azure, not only should you consider what applications or systems you wish to migrate over to Azure but you should also understand the costs associated with the migration.

Microsoft has a tool that will help ease this task for you and its called Azure Migrate. Azure Migrate will help you kick-start your on-premise assessment but estimating the costs for running on-premise machines in Azure.

What the assessment tool does is it calculates the post-migration compute and storage costs based on the recommendations done Azure Migrate for a machine, its disks, and the assessment properties. 

   - **Compute cost:** Using the recommended Azure VM size, Azure Migrate uses the Billing API to calculate the monthly cost for the VM. The calculation takes the operating system, software assurance, reserved instances, VM uptime, location, and currency settings into account. It aggregates the cost across all machines, to calculate the total monthly compute cost.
<br/>
   - **Storage cost:** The monthly storage cost for a machine is calculated by aggregating the monthly cost of all disks attached to the machine. Azure Migrate calculates the total monthly storage costs by aggregating the storage costs of all machines. Currently, the calculation doesn't take offers specified in the assessment settings into account.
Costs are displayed in the currency specified in the assessment settings.

Once the assessment is completed, it will then illustrates it in the following view below a long with the details for each machine.:

![assessment](https://github.com/alvarovitta/Cost-Management/blob/master/Images/assessment-vm-cost.png)

<br/>
<br/>

## Guidance
Use the following guidance in assessing and planning your workloads to Azure.

- Understand [How Azure Migrate Works](https://docs.microsoft.com/en-us/azure/migrate/migrate-overview#how-does-azure-migrate-work)

- When you use Azure Migrate to conduct an assessment of your virtual machines, we recommend that you keep machines with interdependencies within the same project and assessment. If for example, you are using vCenter Server, make sure that dependent machines are in the same folder, datacenter, or cluster for the assessment. 

- Customize the default [assessment properties](https://docs.microsoft.com/en-us/azure/migrate/how-to-modify-assessment#edit-assessment-properties) in Azure migrate as per your requirements

- Before running an assessment, [group machines using machine dependency mapping](https://docs.microsoft.com/en-us/azure/migrate/how-to-create-group-machine-dependencies#prepare-machines-for-dependency-mapping). This will give you a visualization on the dependencies of your machines. This will help you effectively plan your migration to Azure because you will ensure that nothing is left behind and most importantly discover all the interdependent systems that need to migrate together, identify whether a running system is still serving users and/or is a candidate for decommissioning instead of migration.

## Procedure 

- Learn [how to assess your on-premises VMware VMs for migration to Azure](https://docs.microsoft.com/en-us/azure/migrate/tutorial-assessment-vmware)


## Next Steps
See [Designing your Azure Subscription for Cost Management](https://github.com/alvarovitta/Cost-Management/blob/master/New-3.2-Designing-your-Azure-subscription-for-cost-management.md)
