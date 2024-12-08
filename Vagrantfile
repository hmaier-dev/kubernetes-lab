# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "bento/debian-11"

  config.vm.define "main" do |main|
    main.vm.hostname = "k8s-main"
    main.vm.network "private_network", type: "dhcp"
    main.vm.provision "ansible" do |ansible|
      ansible.playbook = "playbook-main.yml"
    end
  end
  
  (1..4).each do |i|
    config.vm.define "worker#{i}" do |worker|
      worker.vm.hostname = "k8s-worker#{i}"
      worker.vm.network "private_network", type: "dhcp"
      worker.vm.provision "ansible" do |ansible|
        ansible.playbook = "playbook-worker.yml"
      end
    end
  end

end
