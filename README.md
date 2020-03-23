# Kubernetes manifests

To apply manifests:
```console
$ kubectl apply ./
```

It will create `Deployment` object, as well as a `Service` with an external IP address.  
To find the external IP address of your application:
```console
$ kubectl get service blockchain-server
```
Then visit the application on your browser to see it running.
