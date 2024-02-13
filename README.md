# Network Automation with Ansible in Virtual Environments and Presentation

## Objective
This group assignment (1-3 students per group) aims to provide hands-on experience in automating network configurations using Ansible within virtual network environments. Groups will create Ansible playbooks for configuring network devices, implement VLANs, configure a routing protocol, use Jinja2 templates, develop an Ansible role, automate deployment with GitHub Actions, and secure sensitive data using Ansible Vault. The project concludes with a group presentation of the deployed lab.

## Group Work and Collaboration
- Each group should have 1-3 members. (Can be done alone too)
- Tasks should be distributed evenly, and members are expected to contribute equally.
- Collaboration will be facilitated through GitHub, leveraging issues, pull requests, and code reviews for quality assurance.

## Requirements
- Setup a virtual network environment using GNS3, Containerlab, or VMs to simulate 3-4 network devices (switches/routers).
- Ansible installed on a control machine.
- Basic understanding of YAML, Jinja2 templates, GitHub Actions, and the chosen network simulation tool.
- A GitHub account.
  
## GitHub Collaboration
- **Repository Setup**: One member should set up a GitHub repository and add other members as collaborators.
- **Branch Strategy**: Use feature branches for development, ensuring that the main branch remains stable.
- **Pull Requests and Reviews**: Members should use pull requests (PRs) for merging changes. At least one other group member must review and approve the PR before merging.
- **Contribution Tracking**: Ensure that each group member's contributions are visible through commits and PRs.

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

## Part 5: Securing Sensitive Data with Ansible Vault
1. Use Ansible Vault to encrypt sensitive information, such as passwords or secret keys, required by your playbooks.
2. Update your playbooks to reference encrypted data, ensuring secure handling of credentials and other sensitive information.

## Part 6: Automating Deployment with GitHub Actions
1. Store your Ansible configurations and encrypted Ansible Vault files in a GitHub repository.
2. Setup a `.github/workflows/ansible-deploy.yml` workflow for automated deployment upon updates to the main branch.

## Part 7: Presentation and Demonstration
- **Prepare a Presentation**: Outline your project, including the choice of virtual environment, network configurations, Ansible playbooks and role, GitHub Actions automation, and the integration of Ansible Vault for security.
- **Live Demonstration**: Demonstrate the automated deployment in your virtual environment, emphasizing how Ansible Vault secures sensitive data.
- **Discussion**: Discuss design choices, challenges, and insights into real-world network management automation with Ansible, focusing on security practices.

## Deliverables
- Ansible inventory files, playbooks, Jinja2 templates, roles, and encrypted Ansible Vault files.
- GitHub repository URL containing your project.
- Presentation and demonstration of your lab deployment.

## Submission Guidelines
- Submit your GitHub repository link containing the project files before the presentation date.
- Present and demonstrate your lab deployment in class, discussing your project insights and the role of Ansible Vault in securing network automation.
- Ensure that the repository reflects contributions from all group members.
