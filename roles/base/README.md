
The *base* role is used to bootstrap and add a passwordless *ansible* user.

- Use ansible-vault to generate the ansible.pub ssh-key : ` ansible-vault encrypt_string --vault-id ssh@../pass/ssh_pass "secret_ssh_key" --name "ssh_key" `
- Copy the resulting string to `roles/base/vars/main.yaml`
- Run the *base* playbook while override the ansible user in ansible.cgf: `ansible-playbook -k --ask-become-pass -u joe` 
