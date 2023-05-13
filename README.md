# Deploy-MongoDB-App-using-K8S
## Prerequisites
- Install a hypervisor in your local PC such as (VMware workstation , virtualbox) for windows
- A Linux, macOS or Windows machine
- At least 2 CPUs and 2 GB of RAM
- Container runtime (Docker)
- Install Minikube and Kubectl


## Here are the basic steps to deploy MongoDB and Mongo Express using Kubernetes:

1. Create a ConfigMap to store the MongoDB configuration.
2. Create a Secret to store the credentials of the mongodb in encrypted form
3. Create a Deployment to run the MongoDB pods. Use the ConfigMap to pass the config to the pods.
4. Create a ClusterIP Service to expose MongoDB within the cluster.
5. Create a Deployment to run the Mongo Express pods.
6. Create a NodePort Service to expose Mongo Express outside the cluster.
7. Access the Mongo Express UI using the NodePort IP and port. You can then manage your database.

In summary:

- Use Secret for encrypting
-  Use ConfigMaps for config
- Deployments for running pods
- ClusterIP Service for internal access
- NodePort Service for external access
- Initialize replica set after deploy
- Access Mongo Express UI to manage database
