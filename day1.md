#Day 1

##### Towards a standardized Application def model for k8s
    app model :
        container
        images
        workloads
        cloud services
        config
        ops behavior
        packaging
        deployment
    use helm to package app model content
    gitops workflow to

    dans un dev env:
        - docker-compose
        - localhost db, cache
    pour prod, must be in k8s
        - ops makes template, healthchecks, security, etc..

    problems with that :
        no clan ownership of various aspects
        inconsistencies across environments
        conflicting issues often found at deploy time

    app model is for entire prod application :
        k8s-style declarative management
        can be used with
            git as a source of truth
            existing tools: helm, flux,
            existing deployment flow

    what to run VS how to run it
