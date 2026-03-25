# linux-playbook

An Ansbile playbook that installs a variety of tools for cybersecurity exercises

## Installing Ansible

```bash
sudo add-apt-repository --yes --update ppa:ansible/ansible
sudo apt install ansible -y
```

## Installing this playbook
Clone the repository

Use the latest stable version on the [releases page](https://github.com/jackrschumacher/linux-playbook/releases)


## General commands

`-v, -vv, -vvv` - Increasing levels of verbosity in the terminal

## `install-packages.yaml`

### Check that packages are installed

Navigate to the `linux-playbook` folder and run the following command:

```bash
ansible-playbook playbooks/install-packages.yaml -K -l "[host]"
```

### Update existing packages

Navigate to the `linux-playbook` folder and run the following command:

```bash
ansible-playbook playbooks/install-packages.yaml -K -e "app_state=latest" -l "[host]"
```

### `web-dev.yaml`
