Vagrant.configure("2") do |config|
    config.hostmanager.enabled = true 
    config.hostmanager.manage_host = true
    
  ### nexus3 vm ###
     config.vm.define "nexus3" do |nexus3|
      nexus3.vm.box = "geerlingguy/centos7"
      nexus3.vm.hostname = "nexus3"
      nexus3.vm.network "private_network", ip: "192.168.56.20"
      nexus3.vm.provider "virtualbox" do |vb|
       vb.memory = "1024"
       end
     end
     
  ### SonarQube vm  ####
    config.vm.define "sonarserver" do |sonarserver|
      sonarserver.vm.box = "geerlingguy/centos7"
      sonarserver.vm.hostname = "sonarserver"
      sonarserver.vm.network "private_network", ip: "192.168.56.21"
      sonarserver.vm.provider "virtualbox" do |vb|
        vb.memory = "1024"
        end
    end
    
  ### jenkins vm  #### 
    config.vm.define "jenkins" do |jenkins|
      jenkins.vm.box = "geerlingguy/centos7"
      jenkins.vm.hostname = "jenkins"
      jenkins.vm.network "private_network", ip: "192.168.56.22"
      jenkins.vm.provider "virtualbox" do |vb|
        vb.memory = "1024"
        end
    end
    
  end
  