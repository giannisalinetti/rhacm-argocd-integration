# Quarkus Getting Started ApplicationSet

This ApplicationSet uses a `clusterDecisionResource` generator. This approach leverages the 
`acm-placement` ConfigMap on the cluster to generate the destination clusters.

The target repository uses Kustomize to generate a configuration overlay for the `prod` environment.

For more informations about the `clusterDecisionResource` generator: https://argo-cd.readthedocs.io/en/stable/operator-manual/applicationset/Generators-Cluster-Decision-Resource/


