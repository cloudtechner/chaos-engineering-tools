## Experiment with Steadybit for EC2 Instance Shutdown


## Overview
This README provides step-by-step instructions for conducting an experiment using Steadybit to simulate and handle the shutdown of an Amazon EC2 instance. Steadybit is a powerful chaos engineering tool that helps you test the reliability and resilience of your systems.

In this experiment, we will simulate an instance shutdown scenario and observe how the system behaves under controlled failure conditions.

## Prerequisites
Steadybit Installation: Ensure that Steadybit is installed and configured in your environment. Refer to the official Steadybit documentation for installation instructions.

AWS Account: You should have an active AWS account with access to the EC2 instances you want to experiment with.

## Steps to Perform the Experiment
1. Configure Steadybit Experiment
1.1. Login to Steadybit:

Open your web browser and navigate to the Steadybit dashboard.
Log in using your credentials.
1.2. Create a New Experiment:

Create a new experiment in Steadybit.
Define the experiment parameters, including the target EC2 instance(s) and the experiment duration.
1.3. Configure Actions:

Configure the actions to be performed during the experiment. For this experiment, set an action to simulate the shutdown of the selected EC2 instance(s).
2. Run the Experiment
2.1. Start the Experiment:

Start the experiment in Steadybit to initiate the simulation.
3. Monitor and Analyze
3.1. Observe Instance Behavior:

Monitor the behavior of the EC2 instance(s) during the experiment.
Note how the system reacts to the simulated shutdown event.
3.2. Analyze Results:

Analyze the experiment results provided by Steadybit.
Evaluate how the system behaved, and identify any issues or improvements needed in your system's resilience.
4. Post-Experiment Steps
4.1. Document Observations:

Document your observations and insights from the experiment.
Note any unexpected behavior, errors, or improvements observed during the experiment.
4.2. Adjust System Configuration (If Needed):

Based on the experiment results, make necessary adjustments to your system configuration or resilience strategies.
Additional Resources




