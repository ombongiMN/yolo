- It is pod where StatefulSets will be implemented because server.yml pulls yolo backend image that containes the mongodb implementation
- Volumes will also be implemented in this file to persist data incase a pod is destroyed

## 4. CREATE server-k8storage.yml

- In this configuration, we add a volumeMounts section to the container configuration, which specifies the name and mount path for the volume.
- We also add a volumes section to the pod template, which defines a PersistentVolumeClaim (PVC) named mongo-data-claim.

## How to Add The Files To kubernetes Cluster

- `kubectl apply -f filename.yml`

### GCP Prerequisties

 - Step 1: Create a New Project

 - Step 2: Need to create a Billing Account

 - Step 3: Link billing account with the project created on step 1

 - Step 4: Enable APIs that will need to run the dataflow on GCP

 - Step 5: Download the Google SDK


### Install gcloud CLI and Configure

Once GCP account is create can install gcloud CLI tool.

The gcloud CLI is part of the [Google Cloud SDK](https://cloud.google.com/sdk/docs). Must [download and install the SDK](https://cloud.google.com/sdk/docs/install) on your system and [initialize it](https://cloud.google.com/sdk/docs/initializing) before using gcloudCLI tool
