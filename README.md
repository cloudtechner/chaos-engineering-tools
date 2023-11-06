[![CloudTechner - ChaosEngineering](https://img.shields.io/badge/CloudTechner-ChaosEngineering-green)](https://)

# Chaos Engineering

<img width="667" alt="image" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/f231578d-fa12-4fef-931b-6d35c5dc08e6">

## What is Chaos Engineering? 

Chaos engineering is the discipline of experimenting on a software system in production in order to build confidence in the system's capability to withstand turbulent and unexpected conditions. Chaos engineering is a disciplined approach to identifying failures before they become outages.

## Face of Chaos Engineering

![image](https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/d674f5c7-4257-4039-b640-a5c1dae47a15)


## What is advantage of chaos engineering?

* **Improved system resilience:** Chaos engineering helps to identify and fix weaknesses in a system before they cause outages in production. This makes the system more resilient to unexpected failures.
* **Reduced downtime:** Chaos engineering can help to reduce the amount of downtime that a system experiences. By identifying and fixing weaknesses in the system, chaos engineering can help to prevent outages from happening in the first place.
* **Improved customer satisfaction:** By reducing downtime and improving system resilience, chaos engineering can help to improve customer satisfaction. Customers are less likely to be frustrated if the systems they use are reliable and available.
* **Increased confidence in the system:** Chaos engineering can help to increase confidence in the system by demonstrating that it can withstand unexpected failures. This can be important for both internal and external stakeholders.
* **Better understanding of the system:** Chaos engineering can help to improve understanding of the system by revealing how it behaves under different failure conditions. This knowledge can be used to improve the system's design and architecture.

## Chaos Engineering Tools

* [Litmuschaos](https://github.com/cloudtechner/chaos-engineering-tools/blob/main/Litmuschaos/README.md)
* [Gremlin](https://github.com/cloudtechner/chaos-engineering-tools/blob/main/Gremlin/README.md)

## Comparison of chaos engineering tool

| Feature | Gremlin | Litmus |
| ---- | ------ | --- |
| Deployment | Cloud-based | On-premises or cloud-based |
| Pricing | Commercial | Free and Commercial |
| Supported platforms | AWS,Azure,GCP,K8s,Bare-metal | AWS,Azure,GCP,K8s,Bare-metal <br />spring boot,VMware | 
| Monitoring tools | Datadog, New Relic, AppDynamics | Datadog, Prometheus, Grafana <br />(Manual installation) |
| Types of experiments | 1.Resource Exhaustion<br />2.The Network is Not Reliable<br />3.Datastore saturation<br />4.DNS Unavailability | 1. Pod chaos<br />2. Node chaos<br />3. Network chaos<br />4. Stress chaos<br />5. vm stop<br />6. Vmware stop<br/>[all chaos list](https://litmuschaos.github.io/litmus/experiments/categories/contents/#generic) |
| Experiment template | No dedicated experiment hub<br/>but 1000+ experimental templates | ChaosHub (Faults:50, Experiments:10) |
| Agent installation | Manual installation required | Automatic installation through Helm chart |
| Catagory |<ul><li>it focus on every resource except start in instances</li><li>we can work with k8s resources as well</li></ul> | <ul><li>Mainly most experiment focused on k8s</li><li>only vm stop type experiment on vm label</li></ul> |
| free and commercial difference | |<table>  <thead>  <tr>  <th>Feature</th>  <th>Free</th>  <th>Commercial</th>  </tr>  </thead>  <tbody>  <tr>  <td>Number of<br/> pre-built<br/>experimental templates</td>  <td>Limited</td>  <td>Unlimited</td>  </tr>  <tr>  <td>Parallel experiment<br/>execution</td>  <td>Limited</td>  <td>Unlimited</td>  </tr>  <tr>  <td>Support for multiple Kubernetes clusters</td>  <td>Limited</td>  <td>Unlimited</td>  </tr>  </tbody>  </table> |

