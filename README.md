# K3S Homelab
This document is a record of steps on my kubernetes journey.    
It can be viewed as a changelog.md highlighting most important changes to this repository. 

# Cluster overview
The homelab runs on a k3s distribution of kubernetes. One control node and 3 worker nodes.
The cluster runs on virtual machines provided by UTM
Each VM runs ubuntu server.
Custom setup for each node is automated with a Ansible playbook.

# Kubernetes journal
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

