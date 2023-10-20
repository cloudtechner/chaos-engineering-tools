[![CloudTechner - ChaosEngineering](https://img.shields.io/badge/CloudTechner-ChaosEngineering-green)](https://)

# Chaos Engineering

<img width="667" alt="image" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/f231578d-fa12-4fef-931b-6d35c5dc08e6">

## What is Chaos Engineering? 

Chaos engineering is the discipline of experimenting on a software system in production in order to build confidence in the system's capability to withstand turbulent and unexpected conditions. Chaos engineering is a disciplined approach to identifying failures before they become outages.

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
| Supported platforms | AWS,Azure,GCP,K8s,Bare-metal | AWS,Azure,GCP,K8s,Bare-metal <br />spring boot,VMware | 
| monitoring | | Need to install manually |
| Types of experiments | 1.Resource Exhaustion<br />2.The Network is Not Reliable<br />3.Datastore saturation<br />4.DNS Unavailability | [all_chaos_list](https://litmuschaos.github.io/litmus/experiments/categories/contents/#generic)<br />1. Pod chaos<br />2. Node chaos<br />3. Network chaos<br />4. Stress chaos<br />5. vm stop<br />6. Vmware stop |
| Experiment template | | ChaosHub (Faults:50, Experiments:10) |
