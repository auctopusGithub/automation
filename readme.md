### Welcome to initial setup of the application

1. Connect to deployment maching using VSCode.

2. Run below commnads on deployment machine:
```bash
sudo apt update && sudo apt upgrade -y && sudo apt install git ansible -y
```

3. Clone automation repository using HTTPS on deployment machine:
```bash
git clone https://github.com/auctopusGithub/automation.git
```

4. Run below commands on deployment machine after cloning repository:
```bash
ansible-playbook automation/configure_ssh.yml 
```
```bash
ansible-playbook automation/master_setup.yml
```
