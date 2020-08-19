#kubecon day 3
####3/10 Simplify your cloud native application packaging and deployments
 - porter.sh

cloud-native contient application mais aussi tous les outils

CNAB cloud native application bundle : techno pour packager des apps , cloud agnostic


####9/10 Introduction to Helm
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
