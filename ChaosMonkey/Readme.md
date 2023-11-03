# Chaos Monkey Guide

![image](https://github.com/cloudtechner/chaos-engineering-tools/assets/87966660/3dc79ad2-51be-4fd7-b072-0fc2d10e6181)


In 2010, Netflix announced the existence and success of their custom resiliency tool called **Chaos Monkey**.

## What is Chaos Monkey?

Chaos Monkey is an ingenious service that promotes the development of resilient services by randomly terminating virtual machine (VM) instances and containers. With the release of Chaos Monkey, it has become even more powerful and tightly integrated with Spinnaker, a leading platform for continuous delivery and cloud management.

In 2010, Netflix decided to move their systems to the cloud. In this new environment, hosts could be terminated and replaced at any time, which meant their services needed to prepare for this constraint. By pseudo-randomly rebooting their own hosts, they could suss out any weaknesses and validate that their automated remediation worked correctly. This also helped find "stateful" services, which relied on host resources (such as a local cache and database), as opposed to stateless services, which store such things on a remote host.

Netflix designed Chaos Monkey to test system stability by enforcing failures via the pseudo-random termination of instances and services within Netflix's architecture. Following their migration to the cloud, Netflix's service was newly reliant upon Amazon Web Services and needed a technology that could show them how their system responded when critical components of their production service infrastructure were taken down. Intentionally causing this single failure would suss out any weaknesses in their systems and guide them towards automated solutions that gracefully handle future failures of this sort.

## What is Chaos Engineering?

**Chaos Engineering** is the discipline of experimenting on a distributed system in order to build confidence in the system's capability to withstand turbulent conditions in production. Chaos Monkey helped jumpstart Chaos Engineering as a new engineering practice. Chaos Engineering is a disciplined approach to identifying failures before they become outages. By proactively testing how a system responds to failure conditions, you can identify and fix failures before they become public-facing outages. Chaos Engineering lets you validate what you think will happen with what is actually happening in your systems. By performing the smallest possible experiments, you can measure, you're able to "break things on purpose" in order to learn how to build more resilient systems.







