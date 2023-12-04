## Experiment with Steadybit for EC2 Instance Shutdown


## Overview
This README provides step-by-step instructions for conducting an experiment using Steadybit to simulate and handle the shutdown of an Amazon EC2 instance. Steadybit is a powerful chaos engineering tool that helps you test the reliability and resilience of your systems.

In this experiment, we will simulate an instance shutdown scenario and observe how the system behaves under controlled failure conditions.

## Features
### Attack Types 
* Network 
   * Package Corruption
   * Delay Traffic
   * BLock Traffic
   * Drop Outgoing traffic
   * Block DNS
   * Limit Bandwidth
* Resource
   * Stress Memory
   * Stress IO
   * Stress CPU
* State
   * Shutdown host
   * Stop Process
   * Time Travel


## Prerequisites
Steadybit Installation: Ensure that Steadybit is installed and configured in your environment. Refer to the official Steadybit documentation for installation instructions.

AWS Account: You should have an active AWS account with access to the EC2 instances you want to experiment with.

## Steps to Perform the Experiment
1. Configure Steadybit Experiment
* Login to Steadybit:
Open your web browser and navigate to the Steadybit dashboard.
Log in using your credentials.
* Create a New Experiment:
    Create a new experiment in Steadybit.
    Define the experiment parameters, including the target EC2 instance(s) and the experiment duration.
* Configure Actions:
    Configure the actions to be performed during the experiment. For this experiment, set an action to simulate the shutdown of the selected EC2 instance(s).
* Run the Experiment
    Start the Experiment:
    Start the experiment in Steadybit to initiate the simulation.
* Monitor and Analyze
    Observe Instance Behavior:
    Monitor the behavior of the EC2 instance(s) during the experiment.
<img width="944" alt="image" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/126565907/7eafb719-cbd3-400d-836d-9490effd01a9">

## Note how the system reacts to the simulated shutdown event.
* Analyze Results:
    Analyze the experiment results provided by Steadybit.
    Evaluate how the system behaved, and identify any issues or improvements needed in your system's resilience.
## Post-Experiment Steps
* Document Observations:
    Document your observations and insights from the experiment.
## Note any unexpected behavior, errors, or improvements observed during the experiment.
    Adjust System Configuration (If Needed):
      Based on the experiment results, make necessary adjustments to your system configuration or resilience strategies.
Additional Resources

## steadybit Kubernetes Agent Helm Chart
 This Helm chart adds the steadybit Agent to all nodes in your Kubernetes cluster via a DaemonSet.
 * Add steadybit Helm repository
   * helm repo add steadybit https://steadybit.github.io/helm-charts
   * helm repo update
 * Create Kubernetes namespace
   * kubectl create namespace steadybit-agent
 * Installing the chart
   * To install the chart with the name steadybit-agent and set the values on the command line run:
     * helm install steadybit-agent --namespace steadybit-agent --set agent.key=STEADYBIT_AGENT_KEY --set cluster.name=CLUSTER_NAME steadybit/steadybit-agent
     * <img width="948" alt="image" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/126565907/79ca028a-db57-4be5-b521-9535250b3f24">

 * Uninstallation
   * helm uninstall steadybit-agent -n steadybit-agent




