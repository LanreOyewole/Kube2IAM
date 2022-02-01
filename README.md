# Kube2IAM
Kube2IAM Implementation for Vanilla Kubernetes Cluster in AWS

This is a simple implementation of Kube2IAM in a non-Production environment. It includes the following artefacts:
- Role for EC2 Instance Profile
- Role for additional S3 bucket
- K8s Deployment manifest for Nginx * 2
- K8s RBAC manifest
- K8s Daemonset manifest for Kube2IAM

All the K8s artefacts deploy into the default namespace for simplicity; except for the RBAC.
You will need enhanced privileges in AWS to create the roles and to access the command line of the EC2 node.
You will also need K8s privileges to deploy the manifests and access the command line of the Pods - to install aws-cli.

Comments/problems/feedback: <a href="https://www.linkedin.com/in/lanreoyewole/">@LinkedIn</a>
