# RHACM ArgoCD Integration

This repository demonstrates how to integrate ArgoCD in the RHACM hub (aka local-cluster), with 
the purpose of natively manage ApplicationSets as first class resources.

To configure the environment create the resources in the **prerequisites** folder and
add the following annotation to the *managedclusters* that must be included in the placement 
with the following label:

```
metadata:
  labels:
    cluster.open-cluster-management.io/clusterset: all-openshift-clusters
```

The ManagedClusterSet `all-openshift-clusters` was choosen for this example and all the clusters
belogint to it will receive a generated ArgoCD application.
