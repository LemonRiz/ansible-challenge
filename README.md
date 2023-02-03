# ansible-challenge

Screen recording of playbook running and Jenkins working.

![Recording](Jenkins%20Playbook.gif)

I created two instances on AWS - one for the Ansible Agent and a JenkinsHost machine.
Had to provision a VM using Vagrant, then used rsync to mount the vm-share folder in the agent instance (in this repo, containing inventory.txt and jenkins-config.yml).

The rsync command can create a shared folder in another machine via its IP address.

SSH into the agent machine and locate the shared folder. CD into the vm-share folder, which contains the files needed to run the Ansible Playbook command:

ansible-playbook -v jenkins-config.yml -i inventory.txt

Once this has completed, I accessed the public IP for the Jenkins Agent machine instanced on Amazon via my browser and using port 8080:

(PUBLICIP):8080

This then will load up the Jenkins app in browser.
