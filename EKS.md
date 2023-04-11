## EKS IN AWS

1. Create an EKS cluster:
  ``` bash
  $ eksctl create cluster --name my-cluster --nodes-min 3 --nodes-max 5 --region us-west-2

  
  ```

2. Update an EKS cluster:

``` bash
$ eksctl update cluster --name my-cluster --version 1.21


```

3. Delete an EKS cluster:

``` bash
$ eksctl delete cluster --name my-cluster


```

4. List EKS clusters:

``` bash

$ eksctl get cluster


```

5. kubectl get nodes

``` bash
$ kubectl get nodes

```

6. Scale worker nodes in an EKS cluster:
``` bash

$ eksctl scale nodegroup --cluster my-cluster --name my-node-group --nodes 4


```


7. Deploy an application to an EKS cluster:

``` bash
 $ kubectl apply -f deployment.yaml



```


8. Expose a service running on an EKS cluster:

``` bash
 
 $kubectl expose deployment my-app --type=LoadBalancer --port=80 --target-port=8080
  
  
```

9. Get logs for a pod running on an EKS cluster:

``` bash
  
  $ kubectl logs my-pod
 
  
```

10. Connect to a pod running on an EKS cluster:
``` bash
  
  $ kubectl exec -it my-pod /bin/bash

```
