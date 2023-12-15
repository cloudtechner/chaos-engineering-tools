<img width="273" alt="image" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/99400e8b-48df-4c58-9186-489f6414b928">


# Azure Chaos studio

Azure Chaos Studio is provided as a service, which means you don’t have to deploy your own infrastructure first to get it up and running. Azure Chaos Studio Preview is a fully managed chaos engineering experimentation platform for accelerating the discovery of hard-to-find problems, from late-stage development through production.

* About: https://learn.microsoft.com/en-us/azure/chaos-studio/
* Tutorial: https://learn.microsoft.com/en-us/azure/chaos-studio/chaos-studio-quickstart-azure-portal
* Azure Chaos studio is SAAS service ((fully managed service by Azure)
* We can use Azure Chaos Studio via azure portal and azure cli and azure chaos packages.
  
# Pricing for Azure Chaos studio

You are charged per minute that an action runs, from start to finish, based on the number of target accounts for your experiment. 

# Agent

* experimental agent-based fault
* experimental service direct fault


# Type of experiments

Documentation link: https://learn.microsoft.com/en-us/azure/chaos-studio/chaos-studio-fault-library

* Azure Cosmos DB chaos: https://learn.microsoft.com/en-us/azure/chaos-studio/chaos-studio-tutorial-service-direct-portal
* Chaos on your virtual machine
* Chaos on AKS
* Dynamic targeting experiment (all vm down of specific zone)
* Chaos Azure Active Directory 

## Aspects
* Time delay
* CPU pressure
* Physical memory pressure
* Virtual memory pressure
* Disk I/O pressure (Windows)
* Disk I/O pressure (Linux)
* Arbitrary stress-ng stress
* Stop service
* Kill process
* DNS failure
* Network latency
* Network disconnect

# List of faults

<img width="128" alt="image" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/df0b52c1-362b-46f7-a167-b893af85e3d1">

<br/>

<img width="145" alt="image" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/d41ca1af-d4f6-43d9-9167-dd59287ff9ed">

# Logging and Monitoring

* Activity log
* Experiment details
* Agent logs

# Limitations

Only supported on a few regions: https://azure.microsoft.com/en-us/explore/global-infrastructure/products-by-region/?products=chaos-studio
Other: https://learn.microsoft.com/en-us/azure/chaos-studio/chaos-studio-limitations

# Example 

1. Create VM

<img width="959" alt="Screenshot 2023-12-14 102544" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/ce77e724-f120-4a40-a806-4adeee9df0c3">

2. Create an experiment template

<img width="951" alt="Screenshot 2023-12-14 102642" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/fbdb05e9-0360-42f3-958b-ed6204bcb524">

3. Provide permission

<img width="745" alt="Screenshot 2023-12-14 102622" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/420d67a4-e166-4bcc-89d4-47a7af26c8cd">

4. Start experiment


