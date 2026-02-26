🚀 Production-Ready CI/CD Pipeline with DevSecOps Practices
This project implements a fully automated CI/CD pipeline designed for secure, reliable, and efficient software delivery. It integrates DevSecOps principles to ensure that automation, security, and observability are built into every stage of the lifecycle — from code commit to production deployment.

<img width="1903" height="1052" alt="image" src="https://github.com/user-attachments/assets/c04cb404-7d3b-4c5d-bc67-2300f8047f67" />
<img width="1183" height="820" alt="image" src="https://github.com/user-attachments/assets/7359233b-4cdf-4110-b15c-9c46eec80e0f" />


⚙️ Pipeline Workflow
1. Code Build & Test

Jenkins triggers the pipeline on every commit push or PR merge.

Source code is compiled and unit tests are executed.

2. Code Quality Analysis

SonarQube scans the codebase for quality issues, code smells, and vulnerabilities.

Quality gates ensure only compliant builds move forward.

3. Security Scanning (DevSecOps Focus)

Docker images are scanned using Trivy for vulnerabilities before deployment.

The build fails if critical or high-severity vulnerabilities are detected.

4. Artifact Management

Validated and secure build artifacts are pushed to Nexus Repository Manager.

5. Deployment to Kubernetes

Jenkins deploys the containerized application to a Kubernetes cluster using deployment manifests or Helm charts.

6. Monitoring & Observability

Prometheus collects performance and health metrics.

Grafana dashboards visualize real-time system performance, error rates, and resource usage.


