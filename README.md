# Kubernetes Helm Charts
Repository for all my helm charts

## Prerequisites

- Docker: For running images and containers
- Kubernetes: For orchestrating multiple docker containers
- kubectl: Command line tool to interact with kube clusters
- helm: Manage the kube packages  

## Useful Commands
- Add repository to Helm - ```helm repo add < any-repository-name > https://prithvi112.github.io/Kubernetes-Helm-Charts```
- Verify all updated chart are present - ```helm search repo < above-repository-name >```
- Install any specific chart - ``` helm install < any-suitable-name > < repository-name >/< chart-name > -f < values yaml file >```  
(The values yaml file will be required for some charts mentioned in table below)
- Update local repository - ```helm repo update < repository-name >```

## Helm Charts
| Type | Chart Name | Purpose | Directory | Values File Required |
|------|------------|---------|-----------|----------------------|
| Platform | Kubernetes Dashboard | Dashboard to monitor kubernetes clusters | kube-dashboard | NO |
| Application | Investment Portfolio | Application to monitor all investments and portfolio | investments-portfolio | YES |
| Platform | System Log Aggregation | Update and perform log analysis on Elasticsearch | system-log-aggregation | YES |
| Application | Jellyfin | Media server for hosting movies and shows | jellyfin | YES |
