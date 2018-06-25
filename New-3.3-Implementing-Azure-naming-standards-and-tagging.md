# Implementing Azure Naming Standards and Tagging

Use the procedure described in this section when applying Azure tags to your subscription. This section also includes examples of common tags you can use as a template upon which to base your organization's requirements. 

<br />
<br />

Apply tags to Azure resources to logically organize them by categories. Each tag consists of a name and a value. Define names and 
values that make the most sense for organizing your subscription. Tags should include 3 types of information:

  - **Billing Information**: cost center, billing ID etc.
  - **Ownership Information**: whom should be contacted when needed
  - **Purpose Information**: environment, application, service


**An example of a common tagging approach:** 

   | __Tag Name__ | __Key__ | __Example__ | __Comment__ |
   |------------------------------|----------------------------|----------------------------|----------------------------|
   | Bill To / Internal Chargeback ID   | billTo  | IT-Chargeback-1234   |  An internal I/O or billing code  | 
   

After you apply tags, you can retrieve all the resources in your subscription with that tag name and value. Tags enable you to retrieve related resources from different resource groups. This approach is helpful when you need to organize resources for billing or management.

<br />
<br />

## Guidance
<br />

### Tag Names: Use the following information when naming your Azure resource tags.

  - Follow [Azure naming rules and restrictions](https://docs.microsoft.com/en-us/azure/architecture/best-practices/naming-conventions#naming-rules-and-restrictions). It is difficult to change a name later. 
  - Names must meet the requirements of their specific resource type 
  - Some types of resources require additional care so follow the [best practices for naming conventions](https://docs.microsoft.com/en-us/azure/architecture/best-practices/naming-conventions)
  - When naming Azure subscriptions, verbose names make understanding the context and purpose of each subscription clear. 
  - When working in an environment with many subscriptions, following a shared naming convention can improve clarity. 
  - Use the following recommended pattern for naming subscriptions:  
Company, Department (optional), Product Line or Service (optional), Environment
      
<br />
<br />

### Tags: Use the following information when designing Azure resource tags: 

   - Each resource or resource group has a maximum of 15 tag name/value pairs. This limitation applies only to tags directly 
   applied to the resource group or resource. A resource group can contain many resources that each have 15 tag name/value 
   pairs. 
   - If you have more than 15 values that you need to associate with a resource, use a JSON string for the tag value. The JSON string 
   can contain many tag values. 
   - Tags applied to the resource group are not inherited by the resources in that resource group. 
   - Use Azure resource policies to apply and enforce mandatory tags across your subscriptions and resource groups to avoid 
   deployment of resources without the required tags 
   - Leverage Tags for purposes of billing monitoring and reporting 
   - Leverage Tags for security and inventory of resources  
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
   
   
## Next steps
[Implementing Azure Cost Management Policies](New-3.4-Implementing-Azure-cost-management-policies.md)
