# arrbor
Ansible Playbook to setup a working basic Jellyfin/*arr environment on a EL based Linux with podman.

## Prerequsities
Install ansible on the server.
```bash
dnf install ansible
```

Make sure podman is installed
```bash
dnf install podman
```

## Installation
1. Clone the Repo
```bash
git clone https://github.com/revresx/arrbor
```

2. (Optional) If using Cloudflare DDNS, make sure to fillout the API-Key and DNS-Zone id in the `arborr-playbook.yaml` file.

3. Run the Playbook
Make sure you user has elevated priviledges. If sudo requieres password run `sudo ls` before running the playbook.
```bash
ansible-playbook arrbor-playbook.yaml
```
