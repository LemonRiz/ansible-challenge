
Virtual Box4
--------------------------------------------------------------

# Vagrant.configure("2") do |config|
#   # Provisiing MongoDB
#   config.vm.define "mongodb" do |mysqldb|
#     mysqldb.vm.box = "generic/ubuntu2010"
#     mysqldb.vm.network "private_network", ip: "192.168.56.20"
#     mysqldb.vm.provider "virtualbox" do |vb|
#       config.vm.synced_folder "env/", "/home/vagrant/env" 
#     end
#     mysqldb.vm.provision "shell", path: "env/mongodb/script.sh"
#   end

  # Provisioning NodeJS App
  config.vm.define "nodeapp" do |nodeapp|
    nodeapp.vm.box = "generic/ubuntu2010"
    nodeapp.vm.network "private_network", ip: "192.168.56.10"
    nodeapp.hostsupdater.aliases = ["nology.training"]
    nodeapp.vm.provider "virtualbox" do |vb|
      
    end
      nodeapp.vm.provision "shell", path: "./jenkins-config.yml"
  end
end