# Target

* Ansible playbook to update, upgrade apt packages and install the APPs I use on my Ubuntu system.

### Caution

1. The playbook is set to run on `localhost` by default. If you want to run it on a different host, change the `hosts` line accordingly.
2. The playbook uses `become: yes` to run tasks with elevated privileges. Ensure you have the necessary permissions and that your user can use `sudo` without a password prompt.
3. Must install Ansible core on your system.

### Execution

```bash
ansible-playbook --ask-become-pass playbook.yml
```
