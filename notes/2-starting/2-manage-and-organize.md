https://portal.azure.com/#view/Microsoft_Azure_Resources/QuickstartTutorialBlade/checklistId/get-started-with-azure/sectionId/get-started-navigating-the-portal/lessonId/get-started-navigating-azure-portal
https://www.youtube.com/watch?v=OEdZGF1JcEI

0. ## Questions I have after watching:
   -
1. ## Summary:
   - Resource groups
   - Tags
2. ## Body
   1. Resource hierarchy
      - like a directory (questionable)
      - Taxonomy - each is one-to-many with the one below:
        - management group
          - So like a company level thing?
        - subscription
          - So like a dept? Things that are billd together?
          - Has a decision guide:
            https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/decision-guides/subscriptions
        - Resource group
          - So like a project / application / svc?
          - Like a bunch of resources that are conceptually the same project
        - Resource
          - Undefined so far. Instance of service?
      - naming conventions are recommended
        - Resource names have restrictions; ex. VMs are limited to 15 chars. Deal with it.
        - Ex: rg-<workload or application>-<region>-<dev/prod>-<counter>
        - Don't encode everything - use tags for most of it
   2. Tagging
      - Tags can be applied to resources, resource groups, and subscriptions
      - Tags are name/value pairs
      - Tags are searchable
