
## Overview 


There are other requirements that Cost Management should consider beyond operations and cloud spend. As more people in the organization use the Azure Cloud Platform, a minimum of three additional tiers of cloud spend management are added to the process: 


 


### Cost Management for Executives 


IT and Business executives in the organization need to ensure that the move to Public Cloud is adding value to the business units in the organization and, most importantly, the Return On Investment (ROI) is optimal. Every new resource added to the cloud has to be connected to added value stream and should reconfirm executives that Public Cloud is the platform of choice. Consider this, the concept of a Business Case for Public Cloud has evolved from a one-time financial exercise into an iterative process that will require to continuously evaluate the financial state of the Public Cloud. This result in additional capabilities beyond reporting and dashboarding, including forecasting and alerting. 


 

### Cost Management for Finance Teams 


Forecasting and budgeting is at the core of the requirements that Finance teams are looking in regards to Public Cloud Spend. The concept that, due to its native capabilities, cloud spending can't be forecasted or budgeted in advanced is a pretty popular myth. Cost Management should address the right capabilities based on analytics and monitoring that will ensure cost spending patterns that can be leveraged for forecasting and budgeting. Cloud is agile and flexible by nature but by no means it is an unpredictable ecosystem. 


 


### Cost Management for Project Teams 


Any project or initiative is focused on delivery the maximum amount of value possible in the timeline and budget that has been given. It is fundamental that every manager that is leveraging the cloud for their own initiative has the right amount of information at the right time to make sure effective decisions are made towards the project and its stakeholders. Project teams can't rely on reactive reporting or date around cloud spend. Quite the opposite. The more close to real-time cloud spend data is provided, the more educated decisions will be made to ensure project completion and value delivery. 


 


 


## Azure (Public Cloud) Metering Overview 


 


The following section will focus on Azure metering from the Infrastructure as a Service (IaaS) and Platform as a Service (PaaS) point of view since it addresses the most complex level of metering and costing. Once you have a better understanding on how metering happens for these two cloud models, we will spend sometimes on the Software as a Service (SaaS) model. 


 


## Resource: the minimum unit for metering 


 


In the Azure Platform ecosystem a "resource" represents the minimum model that can be represented. As a result all metering happens around all the resources that you enable in your Azure environments. Resources have three main properties: A name, a type, and a location. Pricing for each resource is defined based on its type and location.  In addition, all resources also have tagging properties which we will discuss more in detail in the "Chargeback and Showback" section in this document. We will use tagging as our way to add meta-data to each resource that will help us facilitate the process of billing for your organization. 


 


It is important to highlight that this separation model (by resource) it is what will actually help you to optimize your cost in the cloud and achieve economies of scale. You will be charge only for the resources that you use (type), where is that resource located (location) and how long you use it (duration). There is a difference between deploying capabilities and consuming capabilities which we will touch in detail in the billing section. But contrast this with the traditional purchase of an infrastructure component in which, at the moment you procure it, you are accountable for its entire cost regardless on how it is use, where it is and for how long it has been functioning. You could have this component turned off on a shelf and you are still getting the bill for it. 


 


## Important considerations about Azure Resources 
 

  - Resource groups are a collection of resources irrespective of their type. This grouping can be considered a special type of tag
  - Services are also a collection of resources in Azure. However, these are combined to provide a specific cloud capability. e.g., A chatbot is a service in Azure composed of 10 different azure resources 
  - The Azure Resource Manager (ARM) is the main management engine for all azure resources. Every single resource in azure is provisioned, managed and consumed via the ARM as shown in the figure below: 

![ConsistentManagementLayer](https://github.com/alvarovitta/Cost-Management/blob/master/Images/ConsistentManagementLayer.png)
 
  - Azure subscriptions are your highest level of hierarchy and grouping in Azure from the Administrator perspective.  
  - In an Enterprise Agreement setting, there is an additional hierarchy and grouping that includes Enterprise Enrollment, departments and account (see figure below). For more detail on how this is setup, please refer to Link to the foundational documentation created by Alvaro and team


 
![RoleLayers](https://github.com/alvarovitta/Cost-Management/blob/master/Images/RoleLayers.png)
 


## Resource Lifecycle 

In contrast to the traditional IT model, Azure resources have a very distinct lifecycle. In Azure, you can reserve, freeze and shutdown resources, same as resource groups and service, at any given time. e.g., you procure and assigned a physical component to a department in your organization and you will charge that department until the physical component is decommissioned (regardless of usage). If two departments use it then you divide the cost and so on. In Azure, a department in your organization can start the month deploying 100 resources. During day 2 they will freeze have of them, and finish the month with 10 active resources and other 10 frozen. This is the complexity that comes with the traceability and flexibility of resources in Cloud. No day is the same from the perspective of your Azure resource footprint snapshot. 

 


## Resource availability 



One of the most valuable capabilities in the public cloud, is the ability to scale on demand (some call it infinite computing but that is not a real representation even for the public cloud) any resource at any given time. This is a very valuable capability but without the right policy and governance frameworks, it can get out of hand. Via what is known as "Infrastructure as Code" or "Configuration as Code" you can deployed from hundreds to thousands of servers with a single click. A close relationship between Cloud Operations, IT and the business should exist to make sure that cloud consumption aligns with the organizational business and financial goals 


 
