# stateful-deployment

# Point 2  Kubernetes StatefulSet [5 pts]
Write a Kubernetes StatefulSet to deploy the nginx container from the previous question. Utilize persistent volume claims and define resource limits for optimal performance.
 >> statefulset.yaml file that deploys the nginx container and uses CSI driver as storage clase and PVC volumes 
 >> nginx username and password is set as env variable but this can be set in secret file for secure access 

# Point 3. Build a Deployment Pipeline [10 pts]
Set up a streamlined build and deployment pipeline for the nginx application using GitHub Actions or an equivalent CI/CD tool. Ensure the pipeline covers building the Docker image, running security checks, and deploying to a Kubernetes cluster.

>> deploy,yaml triggers when we push the changes to the main branch 

The deployment works when it was deployed in minikube @my local system but deployment fails when 
run on the minikube installed on the runner , that might be because of CSI driver and Pv not boubnd to the volume 

I have used Docker username and password explicitly , as I could create the secrets on DOCKHUB on my private reigtries 
Ideally the username and passoword has to be set as secret variable .
 
