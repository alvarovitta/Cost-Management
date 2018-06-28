# Defining your Cost Management Business Requirements
Use the information described in this section to identify your business requirements.
<br />
<br />

The promise of Publc Cloud is built upon a series of foundational elements such as agility and transformation. However, the cost aspect of public cloud (Cost efficiency, economies of scale, Capex vs. Opex) is one of the main drivers for adoption. While all these benefits can be achieved, it is required to adopt a new mindset compared to the traditional on-premise infrastructure management of cost.
<br />
<br />

## Guidance
Decisions, Tradeoffs and risk should be approached from a different perspective. This section will focus on solving the problem of adopting public cloud from the perspective of cost. With this in mind, the problem that we are trying to solve is <i>"How to do more with less"</i>. To achieve this objective, collaboration between business and technology stakeholders is fundamental. 


**Recognize the motivation to use Public Cloud**:  
It is important to identify the reasons why the organization has decided to adopt Public Cloud. From the cost perspective, these motivations could be linked to: 

- Business/Value Case:  
Organization proactively is looking for public cloud as means to reduce or optimize Capital and Operational Spend. It is important to leverage the business/value case produce as your point of guidance for your cost management strategy. The success of Public Cloud adoption will be measured againts the benefits, success factors and metrics defined in the business/value case

- Compelling Event:  
The organization is reacting to an event that is currently impacting or will impact the value of the organization. Compelling events normally will not prioritize cost management. However, it is important to provide fast and accurate cost information to decision makers to help drive decisions

- Ad-hoc:  
Organizations are considering cloud for specific program/projects that need to leverage the value of cloud. This also includes early experimentation or validation.
<br />
<br />

**Aligning cloud cost with current financial structure**:  
It is fundamental that you align the Azure cost management structure to the current financial structure and process of your organization. 

   - Discuss with the financial teams and people responsible of the Azure cost management what is a suitable financial structure.
   
   - Consider if the organization measure finances by business units (i.e., Lines of Business), cost centres, and/or budget-drived (projects). The early identification of this financial categoriation will be used as direct inputs for your Azure subscription design.
<br />
<br />

**Alignment of performance metrics**:  
Find alignnment to the metrics that already matter to your organization both inside and outside the technology domain. Metrics such as: Total Cost of Ownership (TCO), Return on Investment (ROI), Profit and Loss (PNL) and/or benefit realization coming from the business/value case.
<br />
<br />

**Identifying User Requirements**:  
It is also important to put yourself in the role of the key stakeholders that will be responsible for the cloud cost management. We recommend to focus your requirements based on three categories of cost management stakeholders:
<br />
<br />

**Cost Management for Executives**:  
IT and Business executives in the organization need to ensure that the move to Public Cloud is adding value to the business units in the organization and, most importantly, the Return On Investment (ROI) is optimal. Every new resource added to the cloud has to be connected to added value stream and should reconfirm executives that Public Cloud is the platform of choice. Consider this, the concept of a Business Case for Public Cloud has evolved from a one-time financial exercise into an iterative process that will require to continuously evaluate the financial state of the Public Cloud. This result in additional capabilities beyond reporting and dashboarding, including forecasting and alerting. 
<br />
<br />

**Cost Management for Finance Teams**:  
Forecasting and budgeting is at the core of the requirements that Finance teams are looking in regards to Public Cloud Spend. The concept that, due to its native capabilities, cloud spending can't be forecasted or budgeted in advanced is a pretty popular myth. Cost Management should address the right capabilities based on analytics and monitoring that will ensure cost spending patterns that can be leveraged for forecasting and budgeting. Cloud is agile and flexible by nature but by no means it is an unpredictable ecosystem. 
<br />
<br />

**Cost Management for Project Teams**:   
Any project or initiative is focused on delivery the maximum amount of value possible in the timeline and budget that has been given. It is fundamental that every manager that is leveraging the cloud for their own initiative has the right amount of information at the right time to make sure effective decisions are made towards the project and its stakeholders. Project teams can't rely on reactive reporting or date around cloud spend. Quite the opposite. The more close to real-time cloud spend data is provided, the more educated decisions will be made to ensure project completion and value delivery. 
<br />
<br />

**Technical Considerations - Azure Subcriptions**:  
As mentiomed earlier, as early as possible, ensure that the Subscription hierarchy is reflective of the structure of your organization. Some recommendations include:

 - Azure subscriptions are your highest level of hierarchy and grouping in Azure from the Administrator perspective. Leverage this hierarchy to represent the financial structure of the organization.

 - In an Enterprise Agreement setting, there is an additional hierarchy and grouping that includes Enterprise Enrollment, departments and account (see figure below). For more detail on how this is setup, please refer to Link to the foundational documentation created by Alvaro and team.

 The image below shows the different subscription roles and layers that can be setup as part of your Azure configuration:
<br />
<br />

![RoleLayers](https://github.com/alvarovitta/Cost-Management/blob/master/Images/RoleLayers.png)
<br />
<br />

## Next steps  
[Defining your Cost Management Strategy](1.2-Defining-your-cost-management-strategy.md)
