# LitmusChaos

* Open source cloud native chaos engineering framework

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
