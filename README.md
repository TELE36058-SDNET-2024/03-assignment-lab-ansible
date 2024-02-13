# Network Automation with Ansible in Virtual Environments and Presentation

## Objective
This assignment is designed to immerse students in network automation using Ansible within virtual network environments. It includes creating Ansible playbooks for network configurations, implementing VLANs, configuring a routing protocol, employing Jinja2 templates, developing an Ansible role, automating deployment with GitHub Actions, and concludes with presenting the lab deployment.

## Requirements
- Setup a virtual network environment using GNS3, Containerlab, or VMs to simulate 3-4 network devices (switches/routers).
- Ansible installed on a control machine.
- Basic understanding of YAML, Jinja2 templates, GitHub Actions, and the chosen network simulation tool.
- A GitHub account.

## Environment Setup
Choose one of the following tools for simulating network devices:
- **GNS3**: A graphical network simulator for complex networks.
- **Containerlab**: Simplifies the deployment of network containers as devices.
- **VMs**: Virtual Machines hosting network operating systems or virtualized devices.

## Part 1: Initial Setup and Basic Configurations
1. Prepare your simulation environment with 3-4 network devices.
2. Create an Ansible inventory file with all devices, their IP addresses, and access credentials.
3. Develop `basic_network_setup.yml` playbook for configuring:
   - Unique hostnames.
   - Strong, complex local passwords.
   - SSH and disabling Telnet.
   - Console and VTY access limitations.
   - Logging and timestamps.
   - VLANs for network segmentation.

## Part 2: Routing Protocol Configuration
1. Write `routing_protocol_setup.yml` playbook to configure a selected routing protocol (e.g., OSPF) across devices.

## Part 3: Implementing Jinja2 Templates
1. Generate Jinja2 templates for dynamic device configurations.
2. Update your playbooks to use these templates for configurations.

## Part 4: Developing an Ansible Role
1. Refactor your playbooks into an Ansible role named `network_config` with tasks, handlers, templates, defaults, and vars.

## Part 5: Automating Deployment with GitHub Actions
1. Store your Ansible configurations in a GitHub repository.
2. Setup a `.github/workflows/ansible-deploy.yml` workflow for automated deployment upon updates to the main branch.

## Part 6: Presentation and Demonstration
- **Prepare a Presentation**: Outline your project including the choice of virtual environment, network configurations, Ansible playbooks and role, and GitHub Actions automation.
- **Live Demonstration**: Demonstrate the automated deployment in your virtual environment.
- **Discussion**: Discuss design choices, challenges, and insights into real-world network management automation with Ansible.

## Deliverables
- Ansible inventory files, playbooks, Jinja2 templates, and roles.
- GitHub repository URL containing your project.
- Presentation and demonstration of your lab deployment.

## Submission Guidelines
- Submit your GitHub repository link containing the project files before the presentation date.
- Present and demonstrate your lab deployment in class, discussing your project insights.
