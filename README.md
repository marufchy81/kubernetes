# Kubernetes Cluster Deployment Using KOPS on AWS

This repository contains:
- AWS EC2 instance screenshots
- KOPS-generated Kubernetes cluster details
- Sample deployment YAMLs

## ðŸ“• Screenshots

- **Cluster Configuration**
  ![Cluster Info](kops-cluster/cluster-info.png)

- **EC2 Instances**
  ![EC2 Nodes](kops-cluster/ec2-nodes.png)

## ðŸ“ Deployments

Sample deployment manifests for Kubernetes apps are in the `deployments/` folder.

## ðŸ› ï¸ Tools Used

- **KOPS**
- **AWS EC2 (t2.medium)**
- **S3 Backend for KOPS State Store**

## ðŸ” Exported Environment

```bash
export KOPS_STATE_STORE=s3://july-03-maruf
```

## ðŸ”§ KOPS Commands Used

```bash
kops get cluster
kops update cluster --name <your-cluster-name> --yes --admin
```
