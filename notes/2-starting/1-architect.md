https://portal.azure.com/#view/Microsoft_Azure_Resources/QuickstartTutorialBlade/checklistId/get-started-with-azure/sectionId/get-started-navigating-the-portal/lessonId/get-started-navigating-azure-portal
https://www.youtube.com/watch?v=y8Hy0uYL3hg

0. ## Questions I have after watching:
   - What do you mean 'platforms and technologies'? Is that different jargon for "workloads" or "services"?
   - When you're an internal Azure customer, who is incentivized to reduce "cost"?
   - How do you see the internal cost of a service, compared to the external cost?
1. ## Summary:
   - This is basically a system design interview
   - How to architect solutions
   - How to identify services that you need
   - Eric's experience
   - Standard steps:
     - Identify solutions you need
     - Decompose solution
     - Decide arch style, platforms(?), technologies(?)
       - Means like microservices vs monolith, event driven vs work queue, etc
2. ## Do the thing
   - Buried lead, extracted: Architecture Docs
     - Aka Azure Architecture Center
     - https://learn.microsoft.com/en-us/azure/architecture/
     - Has a central core docs section
       - "Application Architecture Guide"
       - https://learn.microsoft.com/en-us/azure/architecture/guide/
       - The basics of this is
   - Sometimes managers don't know what's possible
     - You suggest ways to "deliver value" and "reduce cost"
   - Hypothetical case:
     - ERP system
       - Old hardware, not supported, outages, scale, etc
     - Brand new e-commerce "solution"
       - Blank canvas
   - Decompose workload:
     - ERP - no need to architect; just replace stuff piecewise
     - E-commerce - needs architecting
       - Will need a compute service for web app
       - Storage service for data
       - Azure Architecture Center (buried lead above)
       - Might have multiple "styles"
         - Means like microservices vs monolith, event driven vs work queue, etc
       - Focus first on "compute", "data", and "messaging
       - We'll use core dotnet microservices with a combination of App Service and Functions Service
         - If we wanted containerization, there's a k8s service
         - If we need more than containerization there's virutal machines
