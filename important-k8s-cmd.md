### Here are some important Kubernetes commands that are commonly used on the master node for cluster management:

#### 1. Cluster Info:

``` kubectl cluster-info``` 
Displays cluster info, such as the URL of the Kubernetes control plane.
#### 2. Check Cluster Nodes:
```kubectl get nodes```
Shows a list of all nodes in the cluster and their statuses.
#### 3. Get All Resources:
```kubectl get all --all-namespaces```
Lists all resources in all namespaces (pods, services, deployments, etc.).
#### 4. Get Pods in a Specific Namespace:
```kubectl get pods -n <namespace>```
List all the pods in a specific namespace.
#### 5. Create Resources:
```kubectl create -f <file>.yaml```
Creates a resource (like pods, deployments, etc.) from a manifest YAML file.
#### 6. Apply Resources:
```kubectl apply -f <file>.yaml```
Applies changes to existing resources or creates them if they don't exist.
#### 7. Describe Resources:
```kubectl describe <resource> <name>```
Provides detailed information about a specific resource (like a pod or service).
#### 8. Get Resource Details:
```kubectl get <resource> <name>```
Shows a brief summary of a specific resource.
#### 9. Delete Resources:
```kubectl delete <resource> <name>```
Deletes a specific resource (e.g., pod, deployment, service).
#### 10. View Logs of a Pod:
```kubectl logs <pod-name>```
Displays the logs of a pod's container.
#### 11. Access a Pod Shell:
```kubectl exec -it <pod-name> -- /bin/bash```
Executes a command inside a running pod, typically used to access the shell.
#### 12. View Resource Utilization (Metrics Server Required):
```kubectl top node```
Shows resource usage (CPU, Memory) for each node in the cluster.
#### 13. Check API Server Status:
```kubectl get componentstatuses```
Shows the status of Kubernetes components like etcd, scheduler, controller-manager, etc.
#### 14. View and Manage ConfigMaps:
```kubectl get configmap```
Lists all the config maps in the current namespace.
```kubectl create configmap <name> --from-literal=<key>=<value>```
Creates a new config map with key-value pairs.
#### 15. Access Control (RBAC) Resources:
```kubectl get roles```
List all roles in the current namespace.
```kubectl get rolebindings```
List all role bindings in the current namespace.
#### 16. View Events in the Cluster:
```kubectl get events```
Displays all the events in the cluster, useful for troubleshooting.
#### 17. View Cluster Role Bindings:
```kubectl get clusterrolebindings```
Displays cluster-wide role bindings (access controls).
#### 18. Check Current Context:
```kubectl config current-context```
Shows the current context (cluster, user, and namespace) being used.
#### 19. Switch Context (Switch Clusters or Users):
```kubectl config use-context <context-name>```
Switches to a different Kubernetes context.
#### 20. Backup/Restore Cluster (via ETCD):
For backups:
```ETCDCTL_API=3 etcdctl snapshot save <file-path>```
To restore:
```ETCDCTL_API=3 etcdctl snapshot restore <file-path>```
These commands are key for managing and troubleshooting your Kubernetes cluster from the master node! Would you like more details on any of these or help with specific commands?



