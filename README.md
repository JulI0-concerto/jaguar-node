### Quick Start
This setup not include nvme disk setup. It lease the nvme disk setup to the operators.
> **_NOTE:_**  Only tested on Ubuntu 22.04.

1. clone the repo and cd into the directory
```bash
git clone https://github.com/JulI0-concerto/jaguar-node.git
```
2. Install ansible
```bash
sudo apt install ansible
```
3. Install ansible community.general module
```bash
ansible-galaxy collection install community.general
````
4. Edit and Run the following command to install the full validator profile
```bash
ansible-playbook  playbooks/full-validator-mainnet-profile.yaml -i inventory -e host=local --connection=local
```