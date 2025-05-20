# K3S Homelab
This document is a record of steps on my kubernetes journey.    
It can be viewed as a changelog.md highlighting most important changes to this repository. 

# Cluster overview
The homelab runs on a k3s distribution of kubernetes. One control node and 3 worker nodes.
The cluster runs on virtual machines provided by UTM
Each VM runs ubuntu server.
Custom setup for each node is automated with a Ansible playbook.

# Kubernetes journal
## [2025-05-08]
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

