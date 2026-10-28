# 🚀 Lab 1: Automated RHEL 10 Hardening & Baseline Configuration with Ansible

This repository contains an **Infrastructure as Code (IaC)** solution designed to deploy a standardized, hardened baseline on **Red Hat Enterprise Linux (RHEL) 10** using **Ansible core**.

---

## 🎯 Objectives
* Automate core system provisioning and baseline configuration on RHEL 10.
* Enforce security best practices (SELinux, Firewalld, SSH Hardening).
* Validate local dry-runs (`--check` mode) before deploying to production-ready target VMs.
* Establish a modular, reusable Ansible role structure (`common_rhel`).

---

## 🏗️ Architecture & Directory Structure

The project follows standard Ansible role design patterns:

```text
homelab/
└── lab1/
    ├── inventory.ini
    ├── site.yml
    └── roles/
        └── common_rhel/
            ├── tasks/
            │   └── main.yml
            ├── handlers/
            │   └── main.yml
            └── meta/
                └── main.yml