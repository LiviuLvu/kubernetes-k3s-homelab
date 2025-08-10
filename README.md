# K3S Experiments
This repository is a personal changelog of Kubernetes experiments running on a small home lab.

## Cluster overview
My homelab runs on a k3s distribution of kubernetes. One control node and 3 worker nodes.  
The nodes run on UTM virtual machines with Linux OS: Ubuntu 24.04 LTS. 
 
Follow my blog for more info about how I use my home lab to run Kubernetes and other tools:
[liviu.pages.dev](https://liviu.pages.dev/)

# Kubernetes journal
## [2025-08-07]
  - CKAD prep: inside a pod run init contaier that downloads a config file in a shared volume
## [2025-08-06]
  - CKAD prep: persistentVolume, persistentVolumeClaim, request pvc for a pod 
## [2025-08-05]
  - CKAD prep concepts: volumeMounts, container securityContext, cronJob
## [2025-08-02]
  - Install headlamp dashboard and make it available on local lan via dns overrides in OPNsense
## [2025-05-31]
  - Use ingress to a service to access a basic deploy
## [2025-05-20]
  - Use service account with admin user to login into kubernetes-dashboard
  - Attempt to access kubernetes-dashboard from outside cluster using ingress
## [2025-05-08]
  - Use configmap to create env variables in pods and volumes
## [2025-05-07]
  - Use cronjobs with limits on start, duration to run repeat tasks at time intervals
  - Create jobs from cronjob
## [2025-05-05]
  - Create job that runs simple command, set nr of completions, parallel runs, limit job time
## [2025-05-04]
  - Create deployments, update image versions, scale replicasets
  - Check rollout status, history, undo deploy
## [2025-05-03]
  - Create a canary deploy
  - Scale the second deploy to 100%, delete the first app v1
## [2025-05-02]
  - Use taint to repel a pod from a node
  - Create node based on nodeSelector and tolerations
## [2025-04-28]
  - Generate yaml file with labeled, annotated pod
  - Edit, add, delete labels and annotations on running pods
## [2025-04-27]
  - Create pod with multiple containers
  - Create pod with initContainers and shared volumes
  - Test access to shared volume on opened port
## [2025-04-26]
  - Run pod with environment variable
## [2025-04-24]
  - Run a task then delete pod automatically
  - View logs from previous pod instance, after a crash restart
## [2025-04-23]
  - Run a command in a pod and view the pod logs with the result
## [2025-04-19]
  - Run commands inside pod, open shell inside pod, install packages
## [2025-04-15]
  - Fixed cluster nodes duplicate ip blocking ingress, created simple ingress controller to provide access inside cluster from local lan
## [2025-04-14]
  - Check k3s available Ingress controller (Traefik, load balancer + api access to services)
  - Forward http requests to services:ports inside cluster
## [2025-04-12]
  - Use port forwarding to make a pod accessible outside cluster
  - Created a deployment with service. Edited service to NodePort with nodePort 32000
## [2025-04-11]
  - Namespace quota limits, manage deployment resources (CPU, MEM, # of Pods). 
## [2025-04-10]
  - Pods, describe pods, generate yaml from command line, multiple container pod use cases

