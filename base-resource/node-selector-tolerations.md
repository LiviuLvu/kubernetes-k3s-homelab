Creates a node that will be assigned to the node named kcontrol, based on the current setup of k3s
Result:
`
k3 get pod -o wide
NAME               READY   STATUS    RESTARTS   AGE     IP           NODE       NOMINATED NODE   READINESS GATES
customerservice1   1/1     Running   0          2m16s   10.42.0.10   kcontrol   <none>           <none>
`
