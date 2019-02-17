# Ansible role for Elasticsearch

This is a simple role that will install Elasticsearch on Debian/Ubuntu from the official APT repo.

It has very basic configuration (see the templates folder).

## Sample playbook

```yaml
---

- hosts: myhost
  roles:
    - name: elasticsearch
      tags: elasticsearch
  vars:
    elasticsearch_jvm_heapsize: 512m
    elasticsearch_network_bind_host: 0.0.0.0
```
