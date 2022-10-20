# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*

- *Analyze costs, scalability, availability, and workflow*

  Cost:
- Generally, App Service costs less than VMs do, especially after introducing the Pay as you go option in App Service.

  Scalability:
- Both approaches have options for scalability, VMs can be grouped together and hence vertically scale.  App Service can be both horizontally and vertically scaled, in a way that is much easier to manage than scaling VMs.

  Availability:
- Both approaches have high availability, however, App Service availability mechanize are automatic, unlike VMs which have an upfront setup of infrastructure.

  Workflow:

  VMs
- *Choose the appropriate solution (VM or App Service) for deploying the app*

  - I went with App Service
- *Justify your choice*

  - For this use case, I chose App Service because:
    - It is a small-scale API, which is well suited for App service
    - App Service costs less overall.
    - There is no need for OS-level control
    - It has a much easier setup, so developers (me) don't need to spend time setting up Docker, Nginx ...etc.

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.*

- If the app intruduced more features that make it a complex API
- If there was a need for system-level control, such as setting up background tasks, need for other applications to run in the same instance, or any special configuration that need control over the OS.
