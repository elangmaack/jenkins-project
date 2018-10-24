Vagrant.configure(2) do |config|
  config.vm.define "jenkins" do |jenkins|
  config.vm.network "forwarded_port", guest: 9000, host: 9900
  config.vm.network "forwarded_port", guest: 8080, host: 8081
      jenkins.vm.box = "ubuntu/trusty64"
      jenkins.vm.network "private_network", ip: "192.168.0.252"
      jenkins.vm.hostname = "jenkins"
      jenkins.vm.provider "virtualbox" do |v|
        v.memory = 4096
        v.cpus = 2
        end
    end
end
