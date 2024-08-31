### Welcome to initial setup of the application

1. Run below commnads on machine:
```bash
  sudo apt update
```
```bash
  sudo apt upgrade
```
```bash
  sudo apt install git ansible -y
```

2. Clone automation repository using HTTPS

```bash
  https://github.com/auctopusGithub/automation.git
```

3. Connect to VS Code

```bash
ansible-playbook -i inventory_file configure_ssh.yml 
```

4. Connect using vscode

5. Clone Linux Deployment Repo

```bash
ansible-playbook -i inventory_file master_setup.yml
```
