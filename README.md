

# Wanderlust Mega Project End to End Implementation


<img src="https://github.com/DevMadhup/Wanderlust-Mega-Project/blob/main/Assets/DevSecOps%2BGitOps.gif" />

#

## Tech stack used in this project:
- GitHub (Code)
- Docker (Containerization)
- Jenkins (CI)
- OWASP (Dependency check)
- SonarQube (Quality)
- Trivy (Filesystem Scan)
- ArgoCD (CD)
- Redis (Caching)
- AWS EKS (Kubernetes)
- Helm (Monitoring using grafana and prometheus)

## Final Workflow Summary:
1. Developers push code to GitHub →Webhook Triggers Jenkins CI/CD pipeline.
2. CI Pipeline:
o OWASP dependency check.
o SonarQube static code analysis.
o Trivy container vulnerability scanning.
o Docker image build & push to registry.

3.CD Pipeline:
o Updates deployment manifests in GitHub.
o ArgoCD deploys the updated application to Kubernetes.
4. Monitoring & Notifications:
o Prometheus & Grafana monitor system performance.
o Jenkins sends email notifications on deployment success or failure
