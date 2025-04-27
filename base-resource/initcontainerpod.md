Creates pod with initContainers and shared volumes

Check events in pod description:
kubectl describe pod initcontainer

Events:
  Type    Reason     Age   From               Message
  ----    ------     ----  ----               -------
  Normal  Scheduled  25s   default-scheduler  Successfully assigned default/initcontainer to knode1
  Normal  Pulling    26s   kubelet            Pulling image "busybox"
  Normal  Pulled     23s   kubelet            Successfully pulled image "busybox" in 2.521s (2.521s including waiting). Image size: 1855985 bytes.
  Normal  Created    23s   kubelet            Created container: busyboxco
  Normal  Started    23s   kubelet            Started container busyboxco
  Normal  Pulling    23s   kubelet            Pulling image "nginx"
  Normal  Pulled     20s   kubelet            Successfully pulled image "nginx" in 2.469s (2.469s including waiting). Image size: 68844367 bytes.
  Normal  Created    20s   kubelet            Created container: nginxco
  Normal  Started    20s   kubelet            Started container nginxco

Test access to volume with:
k3 run initcheck --image=busybox --restart=Never --command --rm -it -o yaml -- wget -O- <initcontainerip>
