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
* Chaosmesh
* Steadybit
* aws-FIS

## Comparison of chaos engineering tool

| Feature | Gremlin | Litmus | ChaosMesh | Steadybit | AWS-FIS |
| ---- | ------ | --- | --- | --- | --- |
| **Deployment** | SAAS | On-premises or SAAS | On-premises | On-premises or SAAS | SAAS (aws only) |
| Pricing | Commercial | Free and Commercial |Free | Commercial | Commercial |
| Supported platforms | AWS,Azure,GCP,K8s,Bare-metal | AWS,Azure,GCP,K8s,Bare-metal <br />spring boot,VMware | AWS, Azure, GCP, Bare-metal | AWS,Azure,GCP Kubernetes, Docker,JVM-based applications,Linux Hosts | AWS and multi AWS accounts |
| Monitoring tools | Datadog, New Relic, AppDynamics | Datadog, Prometheus, Grafana <br />(Manual installation) | Grafana (chaos mesh data source) | Instana, Prometheus, Datadog, New Relic | cloud watch, Event bridge |
| Types of experiments | 1.Resource Exhaustion<br />2.The Network is Not Reliable<br />3.Datastore saturation<br />4.DNS Unavailability | 1. Pod chaos<br />2. Node chaos<br />3. Network chaos<br />4. Stress chaos<br />5. vm stop<br />6. Vmware stop<br/>[all chaos list](https://litmuschaos.github.io/litmus/experiments/categories/contents/#generic) | [k8s](https://chaos-mesh.org/docs/simulate-pod-chaos-on-kubernetes/) , [Physical node](https://chaos-mesh.org/docs/simulate-process-chaos-in-physical-nodes/) | 1.Network: Package Corruption,Delay Traffic,BLock Traffic,Drop Outgoing traffic,Block DNS,Limit Bandwidth<br />2. Resource: Stress Memory,Stress IO,Stress CPU<br />3. State: Shutdown host,Stop Process,Time Travel<br /> | [list](https://github.com/cloudtechner/chaos-engineering-tools/tree/main/aws-FIS) |
| Experiment template | No dedicated experiment hub<br/>but 1000+ experimental templates | ChaosHub (Faults:50, Experiments:10) | NA | NA | Yes, aws Experiment templates |
| Agent installation | Manual installation required | Automatic installation through Helm chart | ChaosMesh agent (Manual), through yml (Automatic) | Agent Installation | Automatic |
| Catagory |<ul><li>it focus on every resource except start in instances</li><li>we can work with k8s resources as well</li></ul> | <ul><li>Mainly most experiment focused on k8s</li><li>only vm stop type experiment on vm label</li></ul> | <ul><li> Experiment focused on k8s </li><li> Experiment focused on Physical nodes </li></ul> | EKS, ECS, EC2 |
| free and commercial difference |<li>only commercial version is available we can use free trial only for 30 days</li> |<table>  <thead>  <tr>  <th>Feature</th>  <th>Free</th>  <th>Commercial</th>  </tr>  </thead>  <tbody>  <tr>  <td>Number of<br/> pre-built<br/>experimental templates</td>  <td>Limited</td>  <td>Unlimited</td>  </tr>  <tr>  <td>Parallel experiment<br/>execution</td>  <td>Limited</td>  <td>Unlimited</td>  </tr>  <tr>  <td>Support for multiple Kubernetes clusters</td>  <td>Limited</td>  <td>Unlimited</td>  </tr>  </tbody>  </table> | Free version only | only enterprise version is avialable free trial only for some days on a account | NA |
| Recommendation | Gremlin is a SAAS tool and easy to configure and use it has a lot of experiments but is expensive. Official documentation is also up to date | Litmus is free and commercial, It is easy to configure and use in both ways self-hosted and as a SAAS. Official Documentation is easy. | ChaosMesh is a free tool, Complex to configure, and average list experiments. The documentation is outdated(chaos integration tools). | Steadybit was not an open-source tool. Steadybit is a platform designed for chaos engineering and reliability testing, helping organizations identify and address weaknesses in their systems before they impact users. It operates as a Software as a Service (SaaS) platform, meaning users can access it through a web interface without needing to install or manage the software on their own infrastructure. | It's SAAS and easy to use but must knowledge of aws iam role and policy as prerequisites. Documentation is easy. A disadvantage is not able to perform cross-cloud platfrom as a target |

