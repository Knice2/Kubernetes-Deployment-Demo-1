## What this does
This repo along with https://github.com/knice2/kubernetesmanifestcode creates a Jenkins pipeline with GitOps to deploy code into a Kubernetes cluster. CI part is done via Jenkins and CD part via ArgoCD (GitOps).

## Jenkins installation
1. Jenkins is installed on EC2. 

2. Install Docker on the EC2 after Jenkins is installed

3. Run `sudo chmod 666 /var/run/docker.sock` on the EC2 after Docker is installed.

4. Install Git on the EC2 by running `sudo yum install git`

### Jenkins plugins

Install the following plugins for the demo.
- Amazon EC2 plugin (No need to set up Configure Cloud after)
- Docker plugin  
- Docker Pipeline
- GitHub Integration Plugin
- Parameterized trigger Plugin

## ArgoCD installation 

Install ArgoCD in your Kubernetes cluster following this link - https://argo-cd.readthedocs.io/en/stable/getting_started/

## How to run!

