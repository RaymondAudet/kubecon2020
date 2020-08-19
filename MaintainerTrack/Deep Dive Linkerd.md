# Deep Dive: Linkerd
Speakers Zahari, Maintainer, Linkerd
_In this session, Zahari Dichev, will focus on lessons learned, how to's, and what the future of Linkerd holds._

### Service mesh overview
good to debug systems, see what's happening and diagnose

linked inject proxy in sidecar containers and all traffic goes through it

### control plane to monitor proxies, management console : 
  - tls certificates for proxy
  - service discovey
  - service profiles (timeout & retries) 
  - dashboard & metrics
  - API interface for cli commants (tap, stat) 

### proxy data plane : 
  - latency aware
  - automatic prometheus metric exports
  - automatic tls
  - on-demand diagnostic tap API  

init container pour setup iprules, et route vers proxy before going in app container

### why multi clusters : 
  - Traffic migration
  - canary deployments
  - different environment (np prep prod)
  - failover 
  
### between two clusters : 
  - must share same tls trust root
### DEMO : 
  - move ui traffic to back from us-east to us-west
  
