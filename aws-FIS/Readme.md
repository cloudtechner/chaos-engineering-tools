<img width="107" alt="image" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/f5eb0fe2-10f8-47f7-88b7-6cb290814eda">


# AWS FIS (Fault Injection Simulator)

A fully managed service for running fault injection experiments on AWS Which makes it easier for you to improve your application's performance, observablity, and resilience.

* About: https://docs.aws.amazon.com/fis/latest/userguide/what-is.html
* AWS official Tutorials: https://docs.aws.amazon.com/fis/latest/userguide/fis-tutorials.html
* AWS SAAS service (fully managed service)
* official documentation: https://docs.aws.amazon.com/fis/
* We can use AWS FIS through aws-cli and aws console.

# Type of experiments
<img width="167" alt="image" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/8347dfac-8ef4-49d1-bb45-03cc0b2f6dba">

## List the AWS FIS actions using the AWS CLI

```
aws:cloudwatch:assert-alarm-state
aws:dynamodb:encrypted-global-table-pause-replication
aws:ebs:pause-volume-io
aws:ec2:api-insufficient-instance-capacity-error
aws:ec2:asg-insufficient-instance-capacity-error 
aws:ec2:reboot-instances
aws:ec2:send-spot-instance-interruptions
aws:ec2:stop-instances
aws:ec2:terminate-instances
aws:ecs:drain-container-instances
aws:ecs:stop-task
aws:eks:inject-kubernetes-custom-resource
aws:eks:terminate-nodegroup-instances
aws:elasticache:interrupt-cluster-az-power
aws:fis:inject-api-internal-error
aws:fis:inject-api-throttle-error
aws:fis:inject-api-unavailable-error
aws:fis:wait
aws:network:disrupt-connectivity
aws:network:route-table-disrupt-cross-region-connectivity
aws:network:transit-gateway-disrupt-cross-region-connectivity
aws:rds:failover-db-cluster
aws:rds:reboot-db-instances
aws:s3:bucket-pause-replication
aws:ssm:send-command
aws:ssm:start-automation-execution
```

* **EC2(instance):** https://docs.aws.amazon.com/fis/latest/userguide/fis-tutorial-stop-instances.html

* **ECS:** https://docs.aws.amazon.com/fis/latest/userguide/ecs-task-actions.html
<img width="259" alt="image" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/88a35dbe-66df-4c45-a060-169136671852">
  
* **EKS:** https://docs.aws.amazon.com/fis/latest/userguide/eks-pod-actions.html
<img width="272" alt="image" src="https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/d893da50-76bd-4cf8-969c-c2af0011f30b">





