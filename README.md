# Overview
Sample Packer & Ansible files for Azure ARM

# Preparation
* Prepare your Resource Group & Storage Account to store your image
* Make "builder/variables.json" file to describe your credentials & identifiers
    * "variables.sample.json" is for your reference
* Make "builder/packer.json" file to describe your packer configuration
    * "ubuntu.json" is for your reference

# How to make your image
1. cd builder
2. packer build -var-file=variables.json packer.json
