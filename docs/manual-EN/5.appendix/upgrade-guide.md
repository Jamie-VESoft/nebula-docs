# Nebula Graph Upgrading Guide

This document describes how to upgrade Nebula Graph. Find the corresponding upgrade guide to your version below.

## Upgrading From Nebula Graph RC3 t RC4

- Stop all the Nebula services
  - Run `scripts/nebula.service stop all` command on each machine
  - Then run `scripts/nebula.service status all` command to confirm all services have exited successfully
- Install the new `rpm` package on each machine
  - Run `https://github.com/vesoft-inc/nebula/releases/tag/v1.0.0-rc4` command to download the package
- Then run `rpm -Uvh nebula-1.0.0-rc4.el7-5.x86_64.rpm` command to install Nebula
- Start Nebula services
  - Run `scripts/nebula.service start all` command on each machine
  - Then run `scripts/nebula.service status all` command to confirm all services have started successfully
- **Reimport your data**
