
![Alt text](image.png)

Chaos Mesh is a CNCF(open source) project for chaos engineering. Chaos mesh dedicated  to Kubernetes chaos experiments. Below are links for more information :

* About: https://chaos-mesh.org/
* source code: https://github.com/chaos-mesh/chaos-mesh
* Offical documentation: https://chaos-mesh.org/docs/


# Installation

Installation guide: https://chaos-mesh.org/docs/production-installation-using-helm/

## Enable or disable permission authentication

`helm upgrade chaos-mesh chaos-mesh/chaos-mesh --namespace=chaos-mesh --version 2.6.2 --set dashboard.securityMode=false`

# Experiments

## Types of chaos experiments
<img width="219" alt="image" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/02720553-e82d-4367-9392-d7fdfc0adf00">

* Kubernetes: https://chaos-mesh.org/docs/simulate-pod-chaos-on-kubernetes/
* Physical: https://chaos-mesh.org/docs/chaosd-overview/

## Tools integration

* Github Action: https://chaos-mesh.org/docs/integrate-chaos-mesh-into-github-actions/ (During POC we found the CRD are not maintained by chaosmesh)
* Datasource for Grafana: https://chaos-mesh.org/docs/use-grafana-data-source/ ( chaos mesh plugin are deprecated due to this https://grafana.com/docs/grafana/latest/developers/angular_deprecation/ )

## Exmaple:

doc link: https://chaos-mesh.org/docs/simulate-pod-chaos-on-kubernetes/

<img width="958" alt="image" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/10e0a140-5357-4bb2-821f-318f09b25ce5">

<img width="489" alt="image" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/5c2669f4-4ffc-47bc-b134-7ea70c01d180">


