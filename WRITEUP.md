# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

As the current Flask application is a lightweight API with simple functionality with respect to storage and content the appliction can be deployed using App service with minimum cost.As this doesnot have multiple applictions, manageable number of users ( event if the count increases in future) this can be completely managed with App service.
Also,App Services cost less than VMs do.
In the current situation, an App Service likely works fine - it can scale vertically to meet different demand levels, and the compute resources needed are well within App Service limits. 
It certainly doesnot require dedicated servers at this point of time.

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 
Unless there is a  vast increase in the number of users, it manages various applications within it,and need for dedicated servers for security reasons.
