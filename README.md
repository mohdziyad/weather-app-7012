<h1>Weather Application Deployment</h1>

Helm is used to deploy application to Kubernetes cluster.

<b>Chart package</b> - weatherchart<br>
/templates/deployment.yaml<br>
/templates/service.yaml<br>
/templates/ingress.yaml<br>

nginx-ingress.yaml - To deploy nginx controller with AWS ALB<br>

Jenkinsfile.build - Jenkins build pipeline to package the helm chart and upload to s3 helm repo<br>

Jenkinsfile.deploy - Jenkins pipeline to install  the helm chart containing deployment, service and ingress yaml to the cluster.