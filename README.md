# task_5

Task 5: Kubernetes Deployment Report
 1. Introduction
 The goal of Task 5 was to understand Kubernetes by deploying, scaling, and exposing an
 application on a local cluster.
 Docker Desktop's Kubernetes cluster was used for this task.
 2. Cluster Setup
 Kubernetes was enabled inside Docker Desktop. kubectl was used to verify the cluster and node
 readiness.
 3. Application Deployment
 An NGINX application was deployed using:
 kubectl create deployment my-app --image=nginx
 Pods were verified using:
 kubectl get pods -o wide
 4. Scaling the Application
 Replicas were increased from 1 to 5 using:
 kubectl scale deployment my-app --replicas=5
 5. Service Creation
 A NodePort service was created to expose the application:
 kubectl expose deployment my-app --type=NodePort --port=80
 NodePort was assigned as 30080, accessible via:
 http://localhost:30080
 6. Logs and Debugging
 Logs were checked using:
 kubectl logs
 7. Outcome
The task successfully demonstrated Kubernetes basics:- Deployment creation- Pod scaling- Service exposure- Accessing the app in browser- Checking logs
 8. Conclusion
 The objective of learning Kubernetes fundamentals was successfully achieved.
 Docker Desktop Kubernetes worked effectively to meet all task requirements
