Vagrant.configure("2") do |config|
  config.vm.box = "terrywang/archlinux"
  
  config.vm.provision "shell", inline: "sudo chmod -R 777 /tmp/"
  config.vm.provision "ansible_local" do |ansible|
    ansible.playbook = "provision_playbook.yml"    
  end
end
