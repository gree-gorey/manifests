# Creating Kubernetes cluster cheat-sheet

Install `kubectl`, a CLI for Kubernetes:
```console
$ gcloud components install kubectl
```
or:
```console
$ sudo apt-get install kubectl
```

Create a Google Kubernetes Engine cluster and make sure `kubectl` is pointing to the cluster:
```console
$ gcloud services enable container.googleapis.com
$ gcloud container clusters create <YOUR_CLUSTER_NAME_HERE> --enable-autoupgrade \
    --enable-autoscaling --min-nodes=1 --max-nodes=3 --num-nodes=1 --zone=<ZONE_OF_YOUR_CHOICE>
$ kubectl get nodes
```
