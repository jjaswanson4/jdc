# Josh's Demos Codebase

This is the codebase for the demos I use routinely, consolidated and available publically.

This is an overhaul/migration of my [patching demo](https://github.com/jjaswanson4/patching-demo) codebase because that grew from just a patching demo into multiple demos built on the same building block. The hope with this repository is to simplify and organize better, but I'm not holding my breath.

# Components

There are three main pieces to this codebase:
1. bootstrap - These playbooks build or teardown the provisioner on an instance of Ansible Controller. They expect Controller to have some basic setup done, such as having a source for execution environments (like an instance of private Automation Hub).
2. provisioner - This is what deploys the demos. Generally speaking, each demo is an instance of Ansible Controller, Red Hat Satellite, and some hosts to make changes against. The provisioner will build these components for you automagically.
3. demo - The actual thing that gets shown off. Designed to be spun up, displayed, interacted with, and then torn down.

# Getting Started
First, you can check the list of available demos [here](DEMOS.md).

# Demo Statuses

| Demo | Provisions | Teardown | Runs |
| ---- | ---------- | -------- | ---- |
| Patching | :heavy_check_mark: | :heavy_check_mark: | :grey_question: |
| IDM-AD Integration | :heavy_check_mark: | :heavy_check_mark: | :x: |
| S4/HANA Deployment | :x: | :x: | :x: |
| Compliance | :x: | :x: | :x: |
| AAP Advanced Architecture | :x: | :x: | :x: |