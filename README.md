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
K8s privileges are required to deploy the manifests and access the command line of the Pods - to install aws-cli.
A prerequisite is AWS S3 access to create the read-only nd read+write buckets - edit the resources with suitable bucket names.

Comments/problems/feedback: <a href="https://www.linkedin.com/in/lanreoyewole/">@LinkedIn</a>, <a href="mailto:lanre@net-technologies.com&subject=Kube2IAm%20Article">@Email</a>
