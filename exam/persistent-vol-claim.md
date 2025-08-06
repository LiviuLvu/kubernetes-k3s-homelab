Create persistent volume, after the volume is created, create pv claim.  
Request the volume for a pod using pvc.  
After the pod is deleted and recreated, the previously created data will be available from the persistedVolume.
