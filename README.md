
# What is Ansible ?

Ansible is an open-source IT automation engine that simplifies and automates tasks like provisioning, configuration management, application deployment,and orchestration, using a human-readable language, YAML, and an agentless approach.


# Key Components of Ansible are:

•	Agentless: Unlike other automation tools, Ansible does not require installing an agent on target systems. It uses SSH (Linux) or WinRM (Windows) for communication.

•	Declarative & Idempotent: You describe the desired state, and Ansible ensures it is maintained.

•	Simple Syntax: Uses YAML for playbooks, making it easy to learn.

•	Scalable & Flexible: Manages thousands of servers from a single control node.

•	Extensible: Supports modules, plugins, and integrations with cloud providers like AWS, Azure, and Google Cloud.

# Why Ansible is used ?

Ansible is used for automating tasks related to configuration management, infrastructure provisioning, application deployment, and orchestration, making it a popular choice for DevOps teams to streamline IT processes and accelerate software delivery. Here’s why Ansible is widely used:

1. Configuration Management: Automates system configuration (e.g., installing software, setting up users, managing services). Ensures all systems remain in a consistent state. Avoids manual errors and configuration drift.

2. Application Deployment: Simplifies deploying applications across multiple servers. Reduces deployment time and human intervention. Supports rolling updates and rollback mechanisms.

3. Infrastructure as Code (IaC): Defines infrastructure using code (YAML-based Playbooks). Allows easy replication, version control, and documentation of configurations.

4. Orchestration: Manages complex workflows across multiple environments.Automates interactions between services (e.g., database setup before app deployment).

5. Security & Compliance: Automates security policies, patching, and compliance checks. Detects and remediates security vulnerabilities.

6. Cloud Automation: Supports AWS, Azure, Google Cloud, and other cloud platforms. Automates provisioning and management of cloud resources.

7. Agentless Architecture: Unlike tools like Puppet or Chef, Ansible does not require installing an agent on managed nodes. Uses SSH (for Linux) and WinRM (for Windows), making it lightweight and easy to use.

# How Does Ansible Work ?

Ansible works by connecting to nodes (or hosts) and pushing out small programs called modules to these nodes. Nodes are the target endpoints servers, network devices, or any computer that you aim to manage with Ansible. Modules are used to accomplish automation tasks in Ansible.

Ansible Architecture Components:

1. Control Node: The machine where Ansible is installed and from which commands and playbooks are executed. It connects to managed nodes using SSH or WinRM. 

2. Managed Nodes (Hosts): The servers, VMs, or cloud instances that Ansible manages. They do not need Ansible installed just SSH or WinRM access.

3. Inventory: A file listing the target systems (IP addresses or hostnames) to be managed. Stored in /etc/ansible/hosts or a custom location.

4. Modules: Predefined scripts that perform tasks like installing packages, copying files, or managing services. Examples: yum, apt, service, copy, file.

5. Playbooks: YAML files defining the automation steps (tasks). Example: Installing and starting a web server. 

6. Tasks: Individual actions within a playbook (e.g., install a package, modify a file).

7. Roles: A structured way to organize playbooks for reusability.
