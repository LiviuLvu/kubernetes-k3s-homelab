# K3S Experiments
This repository is a personal changelog of Kubernetes experiments running on a small home lab.

## Cluster overview
My homelab runs on a k3s distribution of kubernetes. One control node and 3 worker nodes.  
The nodes run on UTM virtual machines with Linux OS: Ubuntu 24.04 LTS. 
 
Follow my blog for more info about how I use my home lab to run Kubernetes and other tools:
[liviu.pages.dev](https://liviu.pages.dev/)

# Kubernetes journal
- CKAD prep: readiness, liveness probes check started and periodical state
- CKAD prep: kustomize patch deployment with env vars from generated secret
- CKAD prep: blue green deployment, service redirect requests to new deploy
- CKAD prep: horizontal pod autoscaler
- CKAD prep: Deployment replicaset, versions rollout, scale up/down 
- CKAD prep: view pods filtered by labels, annotations
- CKAD prep: run multicontainer patterns: ambassador, adapter
- CKAD prep: inside a pod run init contaier that downloads a config file in a shared volume
- CKAD prep: persistentVolume, persistentVolumeClaim, request pvc for a pod
- CKAD prep concepts: volumeMounts, container securityContext, cronJob
- Install headlamp dashboard and make it available on local lan via dns overrides in OPNsense
- Use ingress to a service to access a basic deploy
- Use service account with admin user to login into kubernetes-dashboard
- Attempt to access kubernetes-dashboard from outside cluster using ingress
- Use configmap to create env variables in pods and volumes
- Use cronjobs with limits on start, duration to run repeat tasks at time intervals
- Create jobs from cronjob
- Create job that runs simple command, set nr of completions, parallel runs, limit job time
- Create deployments, update image versions, scale replicasets
- Check rollout status, history, undo deploy
- Create a canary deploy
- Scale the second deploy to 100%, delete the first app v1
- Use taint to repel a pod from a node
- Create node based on nodeSelector and tolerations
- Generate yaml file with labeled, annotated pod
- Edit, add, delete labels and annotations on running pods
- Create pod with multiple containers
- Create pod with initContainers and shared volumes
- Test access to shared volume on opened port
