# Gremlin

![image](https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/99e5c582-1294-4d11-9875-25b13a6ce562)

## Gremlin Chaos Engineering Experiments with AWS EC2 Instances

This repository contains documentation and scripts for conducting chaos engineering experiments using Gremlin on AWS EC2 instances. In this repository, we have performed two experiments: a basic EC2 shutdown experiment and an autoscaling with shutdown experiment. These experiments were conducted using the Gremlin tool to simulate real-world failures and test the system's resiliency.

## Features
### Attack Types 
Gremlin provides a wide range of predefined attack types, such as network partition, CPU hog, memory hog, disk I/O, blackhole, DNS attack, and shutdown. These attacks allow users to simulate different failure scenarios and test how their systems respond under adverse conditions.

### Chaos Engineering Scenarios: 
Gremlin allows users to create and execute chaos engineering experiments based on predefined scenarios. Users can specify the target hosts, choose from various attack types, set the duration and frequency of attacks, and specify criteria for experiment success.

### Safety Checks: 
Gremlin incorporates safety checks and guards to prevent experiments from causing permanent damage. Users can set up safeguards, including preconditions and rollback plans, to ensure that experiments are halted if predefined conditions are met, thereby maintaining the safety and integrity of the system.

### Integration: 
Gremlin integrates with popular cloud providers (such as AWS, Azure, and Google Cloud), container orchestration platforms (like Kubernetes and Docker), and other infrastructure tools. This integration allows users to run chaos experiments in their existing environments and seamlessly integrate Gremlin into their workflows.

### Infrastructure and Application Monitoring: 
Gremlin provides real-time monitoring and visibility into the system's behavior during chaos experiments. Users can view metrics, logs, and other performance indicators to analyze the impact of the chaos and identify areas for improvement.

### Team Collaboration: 
Gremlin offers collaboration features, enabling teams to work together on chaos engineering experiments. Users can share experiments, collaborate on scenarios, and analyze results collectively, fostering teamwork and knowledge sharing.

### API Access: 
Gremlin provides a RESTful API, allowing users to programmatically control and automate chaos experiments. This feature is particularly useful for integrating Gremlin into existing automation pipelines and workflows.

### Role-Based Access Control: 
Gremlin offers role-based access control, allowing organizations to define different levels of access and permissions for team members. This feature enhances security by ensuring that only authorized users can create and manage chaos experiments.

### Documentation and Support: 
Gremlin provides extensive documentation, tutorials, and support resources to help users get started with chaos engineering and make the most out of the platform. This support ensures that users can effectively use Gremlin to enhance the resilience of their systems.

These features collectively make Gremlin a powerful tool for implementing chaos engineering practices and improving the reliability and robustness of applications and infrastructure.

## Gremlin tiers
Gremlin is a commercial product developed and maintained by Gremlin Inc., a company specializing in chaos engineering solutions. While there are open-source tools and frameworks available for chaos engineering, Gremlin itself is a paid service that offers additional features, support, and integrations to organizations looking to implement chaos engineering in their environments.

* [Enterprise] (https://app.gremlin.com/login)

## Gremlin Experiments
### Resource Experiments
  * CPU (Generates high load for one or more CPU cores.)
  * Memory (Allocates a specific amount of RAM.)
  * IO (Puts read/write pressure on I/O devices such as hard disks.)
  * Disk (Writes files to disk to fill it to a specific percentage.)

### State Experiments

  * Shutdown (Performs a shutdown (and an optional reboot) on the host operating system to test how your system behaves when losing one or more cluster machines.)

  * Time Travel (Changes the host's system time, which can be used to simulate adjusting to daylight saving time and other time-related events.)

  * Process Killer (Kills the specified process, which can be used to simulate application or dependency crashes. Note: Process experiments do not work for Process ID 1, consider a Shutdown experiment instead.)

 ### Network Experiments
   Network experiments test the impact of lost or delayed traffic to a target. Test how your service behaves when you are unable to reach one of your dependencies, internal or external. Limit the impact to only the traffic you want to test by specifying ports, hostnames, and IP addresses.

   * Blackhole
   * Certificate Expiry
   * Latency
   * Packet Loss
   * DNS

## Prerequisites

Before running the experiments, ensure you have the following prerequisites in place:

- Gremlin account: Sign up for a Gremlin account at [https://www.gremlin.com/](https://www.gremlin.com/) and obtain your Gremlin API key.

  <img width="925" alt="image" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/126565907/ae08788d-78fd-4942-9f35-194d46d604f7">

- AWS account: You need an AWS account with EC2 instances and Autoscaling groups set up.

## Experiment 1: EC2 Shutdown Experiment

This experiment demonstrates how to simulate an EC2 instance failure using Gremlin. Follow these steps to run the experiment:
Steps:
  ** create Experiment
     <img width="936" alt="image" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/126565907/11d3c11d-d458-4397-bc69-73064caf90c9">


1. **Install Gremlin**: Install Gremlin agent on your EC2 instance(s) that you want to target for the experiment.
      * Access the Team Settings page in the Gremlin web app.
      * Click the Configuration tab.
      * On the Client Configuration File line, click Download to download the file. You'll receive a file named config.yaml.
Optionally, make any additional configurations to the config.yaml file.
      * Install Gremlin Package using the following commands:
        # Add packages needed to install and verify gremlin (already on many systems)
          sudo apt update && sudo apt install -y apt-transport-https dirmngr

        # Add the Gremlin repo
          echo "deb https://deb.gremlin.com/ release non-free" | sudo tee /etc/apt/sources.list.d/gremlin.list

        # Import the GPG key
          sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 9CDB294B29A5B1E2E00C24C022E8EF3461A50EF6

        # Install Gremlin
          sudo apt update && sudo apt install -y gremlin gremlind
   
3. **Create a Shutdown Attack**: Use Gremlin's web interface or API to create a shutdown attack targeting the desired EC2 instance. This will simulate the instance being terminated unexpectedly.

4. **Observe the Impact**: Monitor your application and system behavior during the experiment. Note any disruptions and how your application responds to the instance shutdown.

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

