# jenkins-eks
For deploying jenkins in EKS cluster


Steps performed
==================
* Creating a namespace called jenkins-eks in our cluster for deploying the jenkins into
* Creating a serviceaccount jenkins-admin with necessary permissions
* Creating a local PV for persisting the data on pod restarts
* Jenkins deployment
* Service clusterip for exposing the jenkins via portforwarding
   * kubectl --namespace jenkins-eks port-forward svc/jenkins-service --address 0.0.0.0 8080
* Access the jenkins at localhost:8080
