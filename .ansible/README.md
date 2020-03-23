# Ansible

## Run a playbook
```bash
ansible-playbook ./server_setup.yaml -i ./inventories/dev/hosts --key-file=~/.ssh/lightsail.pem --vault-password-file ~/.ansible/.vault_password
```

## Generate ansible secret
```bash
ansible-vault encrypt_string --vault-password-file ~/.ansible/.vault_password "$SECRET" --name "$KEY"
```
