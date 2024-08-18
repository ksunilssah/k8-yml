# Kubernetes (K8)

<b>kubectl</b> commands

## Pods

Get pods list

`kubectl get pods`

Get pods details

`kubectl describe pod podname wide`

Delete pod

`kubectl delete pod podname`

Start a nginx pod

`kubectl run nginx --image=nginx`

Start nodejs in pod

`kubectl run nodepod --image=node:20`

Create pod with nginx with yml file

`kubectl create -f  ymlfile.yml`

## Node's

Get nodes list

`kubectl get nodes`

Get nodes details

`kubectl describe nodes`

## Replication

Create replication pods

`kubectl create -f replica-contollers/rc-controler.yml`

Get Replicationcontrolers

`kubectl get replicationcontroller`

## ReplicaSet

Get Replicaset

`kubectl get replicatset` or `kubectl get rs`

Delete Replicaset (it also delete the pods under it)

`kubectl delete replicaset replicaname`

Get details of Replicaset

`kubectl describe rs`

Scale pods in Replicaset

`kubectl scale rs ReplicaSetName --replicas=5`

or

`kubectl edit replicaset ReplicaSetName`

## Deployment

Get Deployments list

`kubectl get deployment`

or

`kubectl get deploy`

Get all the info (Deployment, ReplicaSet, Pods)

`kubectl get all`

Get Deployment details

`kubectl describe deploy`

Create deployment pods

`kubectl create -f deployment/deployment.yml`
