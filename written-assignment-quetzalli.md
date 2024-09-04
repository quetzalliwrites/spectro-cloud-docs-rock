# Debug with `kubectl` 

The `kubectl` CLI uses the Kubernetes API to help you communicate with Kubernetes clusters (a group of computing machines that run containerized applications).

`Kubectl` offers various debug commands for diagnosing and resolving issues within your Kubernetes environment. 

The table below explains some useful `kubectl` commands and flags to support you in the debugging process. 

| Command                        | Description                                                                 | Flags      |
|--------------------------------|-----------------------------------------------------------------------------|---------------------|
| `kubectl get`    | Get a list of all available pods (a group of one or more containers) and their status.                                       | `pods --all-namespaces`       |
| `kubectl logs`        | Retrieve the logs for a specific pod. Use this when you must review logs or debug a container. | `-c`, `--all-pods`, `--all-containers`  |
| `kubectl exec`        | Explore a container and review its internal log files or configurations.             | `-c`, `--pod-running-timeout duration` |
| `kubectl debug`       | Create a pod copy that continues to run for troubleshooting, even if the container encounters errors. |  `-c`, `--copy-to string` |


## More Resources
- A comprehensive [reference for using the `kubectl` debug command to manage your application](https://kubernetes.io/docs/reference/generated/kubectl/kubectl-commands#debug).
- A comprehensive [reference for understanding the `kubectl` debug command options](https://kubernetes.io/docs/reference/kubectl/generated/kubectl_debug/).  
