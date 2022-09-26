# File From Target Ansible
Creating files of targeted source


## Usage

### Playbook for Debugging

```yaml
---
- hosts: "localhost"

  vars_prompt:
  - name: listing_folder
    prompt: "What should be the folder to be listed?"

  - name: local_dst
    prompt: "Local destination"

  - name: end_op
    prompt: "Choose 'all' OR 'single'"

  roles:
  - file-from-target
...
```
