# LitmusChaos

Litmus is an open-source Chaos Engineering platform designed to help teams uncover infrastructure weaknesses and potential outages through controlled chaos tests. It provides a user-friendly experience, making Chaos Engineering easy for developers and SREs. Litmus adheres to modern chaos engineering best practices and benefits from community collaboration. Moreover, it's fully open source and hosted by CNCF.

## Features

* Chaos workflows
* Teams
* GitOps
* per organization (cross cloud)
* Public and Private ChaosHubs
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
* [self managed](https://github.com/litmuschaos/litmus)
