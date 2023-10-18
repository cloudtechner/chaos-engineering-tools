# How to deploy self hosted LitmusChaos in kubernetes?

## Install Litmus using Helm

**1.**  Create a Litmus namespace in Kubernetes

```console
$ kubectl create ns litmus
```

**2.** Move to helm chart directory and  Install Litmus

```console
$ cd Litmuschaos/litmus/litmuschaos-helm

$ helm install litmus . --namespace litmus  --create-namespace
```

<img width="747" alt="image" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/a8095c63-f70c-4eb6-ba69-df5429b4c442">

## Access and Login to ChaosCenter Dashboard

**1.** Hit loadbalncer ip with 9091 port. e.g  **<Loadbalncer_ip>:9091**

<img width="483" alt="image" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/dbc368fb-a752-4d48-95c8-b80aace11080">

