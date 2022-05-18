## FeedMe DevOps Engineer Take-Home Assignment

Listed below are the technology stack used for this project CI/CD pipeline and deployment.

### Terraform

- Known for its Infrastructure as Code (IaC).
- Used primarily for a quick and convenient creation of Azure AKS cluster.
- The Terraform config files can be found inside the terraform folder.

### Azure AKS cluster

- The selected platform of deployment.

### Docker and Docker-compose

- Containerization of the apps in the project.
- Used in tangent with Kubernetes.

### Github Actions

- The main CI/CD tool for this project.
- Only triggers if there is any commit pushed to the main branch.
- Mainly used to build docker image + push to the dockerhub and deploy to the AKS cluster.

### Helm Chart

- Used to quickly create pods related to the monitoring stack, which are Prometheus and Grafana.

### NGINX

- Proxy used to configure the communication between FrontEnd and BackEnd inside the cluster.
- Can also be used to redirect the default IP address provided by the LoadBalancer to an owned DNS domain.

### Elastic Search, Logstash, Kibana

- The monitoring stack used for log collection in the kubernetes cluster.
