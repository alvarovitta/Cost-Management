# Assessing your Azure Migration Cost
Use the information and procedure described in this section to assess and plan your workloads in Azure.
<br />
<br />

Consider the costs associated with migrating applications or systems to Azure. Use the Microsoft tool: *Azure Migrate* to assess the scale of workload migration and estimate the costs for running on-premises machines in Azure.

Azure Migrate calculates an estimate of costs associated with the post-migration compute and storage. Estimates are calculated based on  sizing requirements for a virtual machine (VM) and its disks.

Azure Migrate calculates:  
- **Compute cost**: Azure Migrate uses the Billing API to calculate the monthly cost for the VM based on the recommended VM size. The calculation uses variables such as: the operating system, software assurance, reserved instances, VM uptime, location, and currency settings. It aggregates the cost across all machines to calculate the total monthly compute cost. 

  
- **Storage cost**: The monthly storage cost for a machine is calculated by aggregating the monthly cost of all disks attached to the machine. Azure Migrate calculates the total monthly storage costs by aggregating the storage costs of all machines. Currently, the calculation doesn't take offers specified in the assessment settings into account.
Costs are displayed in the currency specified in the assessment settings.

Once the assessment is completed, it will then illustrate the estimated monthly costs for compute and storage for each machine in the following view below:

![assessment](https://github.com/alvarovitta/Cost-Management/blob/master/Images/assessment-vm-cost.png)
<br/>
<br/>

## Preparation

Perform the following activities before you begin the procedure tasks: 

  - Review and understand the [prerequisites](https://docs.microsoft.com/en-us/azure/migrate/how-to-scale-assessment#prerequisites) on what you need to be aware of prior to the assessment
  - Review the [port requirements](https://docs.microsoft.com/en-us/azure/migrate/migrate-overview#what-are-the-port-requirements) for Azure Migrate
  - [Plan your migration projects and discoveries](https://docs.microsoft.com/en-us/azure/migrate/how-to-scale-assessment#plan-your-migration-projects-and-discoveries)

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

