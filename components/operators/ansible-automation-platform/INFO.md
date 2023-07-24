# ansible-automation-platform-operator

Red Hat Ansible Automation Platform is designed to help your organization accelerate, orchestrate and innovate with automation. Scale automation with control and insight. Collaborate across teams. Manage policy and governance. Empower multiple IT domains without slowing down development. With Ansible Automation Platform you can drive business outcomes and unleash the full potential of your teams and technology.

## About this Operator

The Ansible Automation Platform Operator provides for push-button deployments and seamless upgrades of the Platform into your OpenShift environment. Ansible Automation Platform deployments include:
  * Automation controller - Define, operate, scale, and delegate automation across the enterprise.
  * Private automation hub - Synchronize, manage and publish automation content to streamline Ansible code within your organization
  * Platform resource operator - Define, launch, and monitor automation in a cloud-native manner

## How to Install

Use of this Red Hat product requires a licensing and subscription agreement.
Install the Red Hat Ansible Automation Platform operator by following instructions presented when you click the Install button.
You can find additional installation guidance in the install documentation: https://red.ht/AAP-20

## How to Upgrade

Starting with AAP 2.2, the database was upgraded to PostgreSQL 13. It is recommended to take a backup of your deployment before upgrading.
To take a backup, create AutomationControllerBackup and AutomationHubBackup objects for your deployments.
When you are ready to upgrade to the next major or minor version, you can do so by changing the channel.

Note: Namespace-scoped and Cluster-scoped deployments are not compatible.
If you originally installed the AAP Operator from the stable-2.1 channel for example, you will want to upgrade to the next minor version by selecting the stable-2.2 channel.
