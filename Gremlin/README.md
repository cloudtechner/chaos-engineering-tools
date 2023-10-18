# Gremlin

![image](https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/99e5c582-1294-4d11-9875-25b13a6ce562)

## Gremlin Chaos Engineering Experiments with AWS EC2 Instances

This repository contains documentation and scripts for conducting chaos engineering experiments using Gremlin on AWS EC2 instances. In this repository, we have performed two experiments: a basic EC2 shutdown experiment and an autoscaling with shutdown experiment. These experiments were conducted using the Gremlin tool to simulate real-world failures and test the system's resiliency.

## Prerequisites

Before running the experiments, ensure you have the following prerequisites in place:

- Gremlin account: Sign up for a Gremlin account at [https://www.gremlin.com/](https://www.gremlin.com/) and obtain your Gremlin API key.
- AWS account: You need an AWS account with EC2 instances and Autoscaling groups set up.

## Experiment 1: EC2 Shutdown Experiment

This experiment demonstrates how to simulate an EC2 instance failure using Gremlin. Follow these steps to run the experiment:

1. **Install Gremlin**: Install Gremlin agent on your EC2 instance(s) that you want to target for the experiment.
   
2. **Create a Shutdown Attack**: Use Gremlin's web interface or API to create a shutdown attack targeting the desired EC2 instance. This will simulate the instance being terminated unexpectedly.

3. **Observe the Impact**: Monitor your application and system behavior during the experiment. Note any disruptions and how your application responds to the instance shutdown.

## Experiment 2: Autoscaling with Shutdown Experiment

This experiment demonstrates how to test the resiliency of your system when Autoscaling groups are in use. Follow these steps to run the experiment:

1. **Configure Autoscaling**: Set up an Autoscaling group in AWS with a minimum and maximum number of instances configured.

2. **Install Gremlin on Autoscaled Instances**: Install Gremlin agent on instances within your Autoscaling group.

3. **Create a Shutdown Attack**: Use Gremlin to create a shutdown attack targeting instances within the Autoscaling group. Gremlin will intelligently target instances without disrupting the overall availability of your application.

4. **Observe the Autoscaling Behavior**: Monitor how Autoscaling responds to the instance shutdown. Observe if new instances are launched to replace the terminated ones.

## Cleanup

After conducting the experiments, ensure you clean up any resources to avoid unnecessary costs. Terminate any unused EC2 instances, disable Gremlin attacks, and remove the Gremlin agent from your instances.

## Additional Resources

- [Gremlin Documentation](https://www.gremlin.com/docs/): Explore Gremlin's official documentation for more detailed information about using the tool for chaos engineering.

Feel free to modify the experiments, documentation, and scripts to fit your specific use case and requirements. Happy experimenting!

