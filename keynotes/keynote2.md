# Keynote 2
#### Whats new in Kubernetes
fit and finish release 1.18

highlights :
 - hpa controls
 - kubectl debug
   - when exec isn't enough
   - creates an ephemeral container
 - kubectl diff
   - https://kubernetes.io/blog/2019/01/14/apiserver-dry-run-and-kubectl-diff/
   - allow apply --dry-run and diff between current and dry-run version

#### the kubernetes effect
automation culture catches on quickly
 - chatOps and chat bots
 - Razee.io to automate deployment of thousands of clusters

#### how not to wreck the planet
our industry contributes to climate change, 1-2% datacenter vs 2.5% for aviation
kubesprawl, the cluster becomes the unit of deployment instead of the container
utilisation vs elasticity
 - utilisation c'est l'usage
 - elasticity c'est le min / max (hpa)
 - cluster are less elastic than applications, every cluster has overhead
serverless ?
 - knative
 - still runs on cluster
still isolate prod, mais consolider dev staging etc..
zombie workloads :
 - 25 % doing useless work!
 - ramener whitelist !
how? make it easy to do the right thing
 - autodelete on creation, that you can extend
 - gitops, do infra as code
   - spin a cluster it up and down

#### platform team
how to scale a platform
 1. get early adopters
 2. build an MVP
 3. create feature roadmap
 4. Platform as a service >> platform as a silo

#### conclusion



