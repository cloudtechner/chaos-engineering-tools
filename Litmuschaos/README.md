# LitmusChaos

![image](https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/124ebca0-9760-4337-9a88-4a18a6de1554)


Litmus is an open-source Chaos Engineering platform designed to help teams uncover infrastructure weaknesses and potential outages through controlled chaos tests. It provides a user-friendly experience, making Chaos Engineering easy for developers and SREs. Litmus adheres to modern chaos engineering best practices and benefits from community collaboration. Moreover, it's fully open source and hosted by CNCF.

## Features

* Chaos workflows
* Teams
* GitOps
* per organization (cross cloud)
* Public and Private ChaosHubs (template of experiments)
* CLI and GUI
* integrated and interleaved monitoring

## Litmuschaos architecture

<img width="827" alt="image" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/fb3bc0c0-6a95-4f9f-a95f-e300723a41f4">

## Litmuschaos experiments

* Pod chaos
    * Pod failure
    * Container kill
    * Pod autoscale

* Node chaos
    * Node drain
    * Froced Eviction
    * Node restart/Power off

* Network chaos
    * Network Latency
    * Packet Loss
    * Network Corruption

* Stress chaos
    * Pod,Node CPU Hog
    * Pod,NOde Memory Hog
    * Pod,Node Disk stress
    * Pod ephemeral storage fill

* cloud service
    * EKS EC2 termination
    * EBS disk detach
 
## Litmuschaos tiers

LitmusChaos was originally created by ChaosNative (Acquired by Harness) and is a CNCF incubated project from 2022 January onwards.
The listed partners offer enterprise distributions, training, and commercial support for LitmusChaos(Harness Chaos Engineering). There are two tier of litmus chaos tool.
 
* [Enterprise](https://app.harness.io/auth/#/signin)
* [self managed](https://github.com/cloudtechner/chaos-engineering-tools/blob/main/Litmuschaos/litmus/Installation-guide.md)

## Prerequisite for performing experiments

### 1. Make a project in litmus chaos 
<img width="602" alt="image" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/5b983113-4c51-4190-bee3-fb3f31288a22">

* select moudle

<img width="270" alt="image" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/9cf9aeb7-cbb1-4592-857c-632eb9cfddb9">

* choose "Chaos Engineering"

 <img width="451" alt="image" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/36afd7b3-1b7f-4241-a275-adc601181ba7">


<br />

### 2. Create environment
<img width="695" alt="image" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/2eb3c853-1ba3-4aa4-b5a1-acf6ff22517f">

<br />

### 3. Create chaos( Connect with infra which you want to perform experiments)
<img width="527" alt="image" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/4b188bdb-830c-4993-b776-e04cb2e8a50d">

<br />
<br />

## Experiments and Steps to perform

* [pod delete](https://github.com/cloudtechner/chaos-engineering-tools/blob/main/Litmuschaos/pod-delete.md)
* [node drain](https://github.com/cloudtechner/chaos-engineering-tools/blob/main/Litmuschaos/node-drain.md)
* [node cpu hog](https://github.com/cloudtechner/chaos-engineering-tools/blob/main/Litmuschaos/node-cpu-hog.md)
* [node memory hog](https://github.com/cloudtechner/chaos-engineering-tools/blob/main/Litmuschaos/node-memory-hog.md)
