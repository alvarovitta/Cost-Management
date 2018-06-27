# Implementing Azure Naming Standards and Tagging
Use the information and procedure described in this section to apply Azure tags to your subscription. 
<br />
<br />

Apply tags to Azure resources when you need to group your billing data. A tag consists of a name and value.  
For example:   
- **"costCenter:finance"**, 
- **"env":"prod"**. 

In the above example, there are two tags applied to a resource. The first tag, "**costCenter:finance**" groups the usage by cost center. The second tag, "**env":"prod**" categorizes the cost by environment, in this case production. 
<br />
<br />

You can define as many tags as needed to categorize your Azure resources however, you will need to define a tagging standard to ensure consistent traceability and categorization of resources. Ensure that the standard is followed by all key stakeholders in your organization.

When you download the usage CSV for services that support tags with billing, the tags appear in the Tags column. See the example below:

![billing](https://github.com/alvarovitta/Cost-Management/blob/master/Images/billing_csv.png)
<br />
<br />


After you apply tags, you can retrieve all the resources in your subscription using a tag name and value. Use tags to retrieve related resources from different resource groups. 
<br />
<br />

## Guidance
Use the Tag Name and Tag Design approach described below for your Azure resource tags.

**Tag Names**:  
Use the following approach when naming your Azure resource tags.

  - Follow [Azure naming rules and restrictions](https://docs.microsoft.com/en-us/azure/architecture/best-practices/naming-conventions#naming-rules-and-restrictions). It is difficult to change a name later. 
  - Names must meet the requirements of their specific resource type 
  - Some types of resources require additional care. Follow the [best practices for naming conventions](https://docs.microsoft.com/en-us/azure/architecture/best-practices/naming-conventions)
  - When naming Azure subscriptions, use verbose names to clarify the context and purpose of each subscription. 
  - When working in an environment with many subscriptions, follow a common naming convention to improve clarity. 
  - Use the following recommended pattern for naming subscriptions:  
    - Company 
    - Department (optional)
    - Product Line or Service (optional)
    - Environment
<br />

**Tag Design**:  
Use the following approach when designing Azure resource tags: 

   - Each resource or resource group has a maximum of 15 tag name/value pairs. This limitation applies only to tags directly 
   applied to the resource group or resource. A resource group can contain many resources; each having 15 tag name/value 
   pairs. 
   - If you have more than 15 values to associate with a resource, use a JSON string for the tag value. The JSON string 
   can contain many tag values. 
   - Tags applied to the resource group are not inherited by the resources in that resource group. 
   - Use Azure resource policies to apply and enforce mandatory tags across your subscriptions and resource groups. Use this approach to avoid deploying resources without the required tags. 
   - Use Tags for billing monitoring and reporting purposes
   - Use Tags for resource security and inventory purposes  
   - The length of tag names are limited to 512 characters, and the tag value is limited to 256 characters. For storage accounts, the tag name is limited to 128 characters, and the tag value is limited to 256 characters. 
   - For further information on tags, see: [Use tags to organize your Azure resources](https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-group-using-tags)
<br />
<br />

## Procedure: How to implement Azure naming standards and tagging 
Use this procedure to create Azure tags using the Azure Portal, PowerShell, or ARM templates. 

1. **Sign into the Azure portal**  
  Login as the Subscription Owner, see:  [Azure Portal](https://portal.azure.com) 

2. **Add a tag to a virtual machine (VM) in Azure**   
  Refer to the following: 
   - [Tagging through the portal](https://docs.microsoft.com/en-us/azure/virtual-machines/windows/tag#tagging-through-the-portal) 
   - [Tagging with PowerShell](https://docs.microsoft.com/en-us/azure/virtual-machines/windows/tag#tagging-with-powershell)
   - [Tagging a virtual machine through templates](https://docs.microsoft.com/en-us/azure/virtual-machines/windows/tag#tagging-a-virtual-machine-through-templates) 
<br />
<br />   
   
## Next steps
[Implementing Azure Cost Management Policies](3.4-Implementing-Azure-cost-management-policies.md)
