## How to Deploy in K8s environment

You may use the following commands:

1. kubectl apply -f feed-deployment.yaml
2. kubectl apply -f feed-service.yaml
3. kubectl apply -f users-deployment.yaml
4. kubectl apply -f users-service.yaml
5. kubectl apply -f frontend-deployment.yaml
6. kubectl apply -f frontend-service.yaml
7. kubectl apply -f reverseproxy-deployment.yaml
8. kubectl apply -f reverseproxy-service.yaml
9. Autoscaling - kubectl autoscale deployment reverseproxy --cpu-percent=50 --min=1 --max=4
10. kubectl port-forward service/reverseproxy 8080:8080
11. kubectl port-forward service/frontend 8100:8100

You may run your app in browser on localhost:8100