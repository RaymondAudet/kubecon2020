# DevOps Patterns and Antipatterns for Continuous Software Updates
Speakers Baruch Sadogursky, Kat Cosgrove
_So, you want to update the software for your user, be it the nodes in your K8s cluster, a browser on user’s desktop, an app in user’s smartphone or even a user’s car. What can possibly go wrong? In this talk, we’ll analyze real-world software update failures and how multiple DevOps patterns, that fit a variety of scenarios, could have saved the developers. Manually making sure that everything works before sending update and expecting the user to do acceptance tests before they update is most definitely not on the list of such patterns. Join us for some awesome and scary continuous update horror stories and some obvious (and some not so obvious) proven ideas for improvement and best practices you can start following tomorrow._

#### why we upgrade softwares?
 - we want new features
   - we update more and more often, smaller but faster
 - for security reasons 
   - stopping distances similarities (identify , fix, deploy)
   - the more we wait, the bigger it gets

#### delivery performances :  
  - to mesure how can we deliver faster and more stable 
  - only 20% are elite

#### question to ask when updating:
 - do we want it? is there any high risk? Do we trust the update? 

#### keypoints : 
 - staging environment needs to die
   - cost to much to maintain
 - should deploy and test in production
 - do less batch updates
 - you should always be able to rollback
 - progressive delivery
   - release only to small batch of user (canary)
 - monitoring, dont rely on user to tell you the problem
 - use feature flags to disable buggy feature if needed
 - zero downtime update (small and frequent)

#### questions : 
 - how to test rollbacks?
   - work more on observability, don't rely on user
 - changelog verbosity
   - don't give too much info in changelog, could be overwhelming
   - have it available, but don't include everything
 - database migrations for canary
   - you can automate DB migrations and schema