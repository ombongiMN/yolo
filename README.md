How to deploy MERN Stack on Google Kubernetes Engine(GKE)

GKE is GCP managed Kubernetes solution that lets you run and manage containerized applications in the cloud.

## Objectives 

1: Dockerize the app and push the images to Google container registry

2: Run the app on GCP GKE

3: Build the kubernetes cluster on GCP GKE

4: Access  clusters from outside

5: Configure Kubectl with GKE Cluster

## To set up the MongoDB have; A StorageClass, A Headless Service and StatefulSet

The Storage class tells Kubernetes what kind of storage to use for the database nodes. On Google Cloud Platform storage choices are SSDs and hard disks

Headless Service doesnt allocate IP address or forward traffic. When combined with statefulSets they can give you unique DNS addresses that let you directly access the pods