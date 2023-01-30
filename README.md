# ansible-challenge

Challenge: Creating a Jenkins Instance with Ansible
For this challenge we would like you to setup / configure a Jenkins instance on AWS
You already have you Ansible agent running and a EC2 machine that you can configure for Jenkins (Rename from JSHost to JenkinsHost)
You will need to have a GitHub repo with the following files:
jenkins-config.yml
inventory.txt
README.md
Deliverables
Playbook for Jenkins
To configure a Jenkins instance on AWS (Provide IP Address)
Detailed README.md on how to use your Playbook.
Screen recording of you playbook running and Jenkins working.

rsync -aP vm-share ssh -i "MehdiRizvi-awskey.pem" ansible-challenge ubuntu@whatever:/home/ubuntu/playbooks/jenkins (for LATER)

ssh -i "MehdiRizvi-awskey.pem" ubuntu@10.0.1.47
