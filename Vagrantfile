Vagrant.configure("2") do |config|
    config.vm.box = "centos/7"
    config.vm.network "private_network", ip: "192.168.56.64"
    config.vm.define "centos7" do |node|
       node.vm.hostname = "centos7"
       node.vm.provision "ansible" do |ansible|
         ansible.playbook = "main.yml"
       end
     end
   end  