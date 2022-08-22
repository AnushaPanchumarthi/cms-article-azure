# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*
|                      | Virtual Machine( Single Tier) Basic Linux  | App Service(Linux Basic) | Comments
| -------------------- | ------------------------------------------ |------------------------- | -------------
| Pricing (per month)  | ₹10,328.20                                 | Monthly: ₹1,049.92       | VMs are highly expensive
| Scalability          | Virtual Machine Scale Sets and Load Balancers | Vertical or Horizontal scaling . Maximum of 14GB of memory and 4 vCPU cores per instance | VMs are highly scalable
| Availability         | 99.95%                                     | 99.95%                   |    Both VMs and App Service give high availability 

As the current Flask application is a lightweight API with simple functionality, so with respect to storage and content the appliction can be deployed using App service with minimum cost.As this doesnot have multiple applications nd manageable number of users ( event if the count increases in future) this can be completely managed with App service provided these are less expensive.
In the current situation, an App Service likely works fine - it can scale vertically to meet different demand levels, and the compute resources needed are well within App Service limits. 
It certainly doesnot require dedicated servers at this point of time.

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

Unless there is a  vast increase in the number of users, it manages various applications within it,and need for dedicated servers for security reasons.
