### Welcome to initial setup of the application

1. Connect to deployment maching using VSCode.

2. Run below commnads on deployment machine:
```bash
sudo apt update && sudo apt upgrade -y && sudo apt install git ansible net-tools -y
```

3. Clone automation repository using HTTPS on deployment machine:
```bash
sudo git clone https://github.com/auctopusGithub/automation.git
```

4. Environment Variable required for Controller:
```bash
export GITHUB_TOKEN=''
export DOCKER_TOKEN=''
export DEPLOYMENT_TYPE='controller'
export SERVER_IP='IP'
export SERVER_PORT='80'
export GITHUB_USERNAME=''
export DOCKER_USERNAME=''
export ANSIBLE_SSH_USER=""
export ANSIBLE_SSH_PASS=""
export ANSIBLE_BECOME_PASS=""
export AUCTOPUS_DOCKER_REPO_URL=""
```

5. Environment Variable required for Runner:
```bash
export GITHUB_TOKEN=''
export DOCKER_TOKEN=''
export DEPLOYMENT_TYPE='runner'
export SERVER_IP='IP'
export SERVER_PORT='8000'
export GITHUB_USERNAME=''
export DOCKER_USERNAME=''
export ANSIBLE_SSH_USER=""
export ANSIBLE_SSH_PASS=""
export ANSIBLE_BECOME_PASS=""
export AUCTOPUS_DOCKER_REPO_URL=""
```

6. Run below commands on deployment machine after cloning repository:
```bash
ansible-playbook automation/master_setup.yml
```
