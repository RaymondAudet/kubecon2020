#### 9/10 Introduction to Helm
_CNCF Helm is a package manager for Kubernetes manifests that helps you write, share, find, and manage applications on Kubernetes. In this session you will learn the basics of Helm. We’ll dive into the components that make up Helm, and what a Helm Package looks like. We’ll then look at ways you can share Helm Charts and we’ll show you how to deploy an existing Helm Chart as well as how to get started writing your own Helm Chart. We’ll finish off by talking about some of the other exciting tools in the Helm ecosystem._


 - https://helm.sh/

helm == apt, yum, brew
easy install, easy upgrade with charts, rollbacks by rollingFront a previous version

kind cluster (kubernetes in docker)
    helm install, uninstall, list
catalog of charts :
    helm repo add sonatype https//nexus3/helm3-charts

helm v3, whats new
 - no more tiller, using k8s api
 - library charts (define elements to be used by other charts)
