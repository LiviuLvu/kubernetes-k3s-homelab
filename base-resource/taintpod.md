After creating a taint on a node:
`kubectl taint node nodename1  tier=frontend:NoSchedule
The taintnode.yaml creates a pod that is accepted by nodename1.

Other created pods that dont specify the taint will be repeled by nodename1.
