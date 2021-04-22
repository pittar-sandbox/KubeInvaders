# OpenShift Deploy with Kustomzie

First, update the route host:

```
export TARGET_NAMESPACES=target-namespace1,target-namespace2
export ROUTE_HOST=kubeinvaders.apps.mycluster.com

sed -i '' "s/kubeinvaders_route_host/$ROUTE_HOST/g" kubeinvaders-dc.yaml

sed -i '' "s/kubeinvaders_route_host/$ROUTE_HOST/g" kubeinvaders-route.yaml
```