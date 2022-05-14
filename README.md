## FeedMe DevOps Engineer Take-Home Assignment

Listed below are the technologies stack used for the project CI/CD pipeline and deployment.

### Terraform

- Known for its Infrastructure as Code (IaC).
- Used primarily for quick and convenient creation of Azure AKS cluster.
- The Terraform config file can be found inside the terraform folder.

### Azure AKS cluster

- The platform of deployment chosen.

### Docker and Docker-compose

- Containerization of the apps in the project.

### Github Actions

- The main CI/CD tool for this project.
- Only triggers if there is any commit push to the main branch.
- Mainly used to build docker image + push to the dockerhub and deploy to the AKS cluster.

### Helm Chart

- Used to quickly create pods related to the monitoring stack, which are Prometheus and Grafana.

### NGINX

- Proxy used to configure the communication between FrontEnd and BackEnd inside the cluster.
- Can also be used to redirect the default IP address provided by the LoadBalancer to an owned DNS domain.

### Prometheus and Grafana

- The monitoring stack chosen to monitor the metric data collection and metric visualizations in the kubernetes cluster.
- The metrics includes CPU, memory and storage of the cluster.
