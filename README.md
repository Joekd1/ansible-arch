
## bootstrapping:

*base* role is used to bootstrap and add a passwordless *ansible* user.

- Use ansible-vault to add the ansible.pub ssh-key : ` ansible-vault encrypt_string --vault-id ssh@../pass/ssh_pass "secret_ssh_key" --name "ssh_key" `
- Copy the resulting string to `roles/base/vars/main.yaml`
- Override the ansible user in ansible.cgf: `ansible-playbook -k --ask-become-pass -u joe` 

