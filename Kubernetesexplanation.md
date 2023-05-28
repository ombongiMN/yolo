- It is pod where StatefulSets will be implemented because server.yml pulls yolo backend image that containes the mongodb implementation
- Volumes will also be implemented in this file to persits data incase a pod is destroyed

## 4. CREATE server-k8storage.yml

- In this configuration, we add a volumeMounts section to the container configuration, which specifies the name and mount path for the volume.
- We also add a volumes section to the pod template, which defines a PersistentVolumeClaim (PVC) named mongo-data-claim.

## How to Add The Files To kubernetes Cluster

- `kubectl apply -f filename.yml`