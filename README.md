Terraform Interview Notes (IaC)

📌 Overview

This repository contains Terraform Infrastructure as Code (IaC) interview notes, covering core concepts, best practices, and commonly asked interview questions.
It is intended for DevOps engineers, cloud engineers, and Terraform learners preparing for interviews.

📘 What is Infrastructure as Code (IaC)?
Infrastructure as Code (IaC) is the practice of managing and provisioning infrastructure using code and templates instead of manual processes.
🔧 Popular IaC Tools

Terraform
Pulumi
OpenTofu
AWS CloudFormation
Azure ARM Templates
GCP Deployment Manager (CDM)


🌍 Terraform & Pulumi
Terraform

Declarative IaC tool by HashiCorp
Uses HCL (HashiCorp Configuration Language)
Cloud‑agnostic (AWS, Azure, GCP)

Pulumi

IaC using general‑purpose languages

Python
Go
TypeScript



✅ Terraform is widely used due to its simplicity and multi‑cloud support.

✅ Why Use IaC? (Benefits)

Cost reduction
Faster infrastructure deployment
Reduced human errors
Improved infrastructure consistency (Idempotency)
Eliminates configuration drift
Easy collaboration and reuse across teams

⭐ Key Interview Keyword
Idempotency → Running the same Terraform code multiple times produces the same result.

📂 Terraform State File
Terraform uses a state file (terraform.tfstate) to track real infrastructure.
State File Stores:

Current infrastructure status
Resource metadata
Timestamps
Who made changes
Which resources/files were modified

💡 Interview Tip:
The state file enables Terraform to decide what to create, update, or delete.

⚖️ Declarative vs Imperative Approach
Declarative Method (Terraform ✅)
You define WHAT you want, not HOW to do it.
Example Requirements:

10 servers
32 GB RAM
16 vCPUs
100 GB storage

Terraform automatically handles the execution steps.
✅ Simple
✅ Less error‑prone
✅ Preferred for IaC

Imperative Method ❌
You define step‑by‑step instructions.
Examples:

Bash / PowerShell scripts
Python scripts
Ansible playbooks

❌ Complex
❌ Requires detailed scripting
❌ Needs high‑skilled engineers
👉 Terraform follows the Declarative approach.

🏗️ Provisioning vs Configuration Management
Provisioning
Creating infrastructure resources:

Virtual Machines
Storage
Network
Load Balancer
Databases

Tools: Terraform, CloudFormation

Configuration Management
Performed after provisioning:

Install software
Configure servers
Maintain systems

Tools:

Ansible
Chef
Puppet
SaltStack

👉 Terraform is mainly a provisioning tool.

🔄 Mutable vs Immutable Infrastructure
Mutable Infrastructure ❌

Existing servers are updated
Software patches applied on the same server
Changes accumulate over time

Problems:

Hard to rollback
Configuration drift
Security risks


Immutable Infrastructure ✅

Servers never change after deployment
Any change creates a new version
Old servers are replaced

Advantages:

Easy rollback
No configuration drift
More secure

💬 Interview Line:

Immutable infrastructure promotes consistency and reliability by replacing infrastructure instead of modifying it.


🛠️ Tools Used with Immutable Infrastructure

Virtualized Platform → Packer (golden images)
Containerized Platform → Docker (container images)


📋 Popular IaC Tools (Interview List)

Terraform
Pulumi
OpenTofu
AWS CloudFormation
Azure ARM Templates
GCP Deployment Manager


❓ Common Terraform Interview Questions
Q: Why Terraform over CloudFormation?

Multi‑cloud support
Reusable modules
Strong community
Simple HCL syntax


Q: What is Idempotency?
Running Terraform multiple times results in the same infrastructure state.

Q: What causes Configuration Drift?
Manual changes made outside Terraform.
✅ Terraform detects drift using the state file.

Q: Is Terraform mutable or immutable?
Terraform supports both, but is mostly used with immutable infrastructure patterns.

✅ One‑Line Interview Summary

Terraform is a declarative, cloud‑agnostic Infrastructure as Code tool that provisions infrastructure efficiently, ensures consistency, eliminates drift, and supports immutable infrastructure practices.


🚀 Who Should Use This Repo?

DevOps Engineers
Cloud Engineers
Terraform Beginners
Interview Preparation Candidates


📌 Next Improvements

Add Terraform code examples
Add AWS real‑world scenarios
Add interview Q&A PDF
Add Terraform state & remote backend examples


✅ Feel free to fork, star, or contribute!

If you want, I can:
