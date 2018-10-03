Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"
  config.vm.define "Haproxy"
  #Example of ansible provisioner
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "haproxy.yml"
    ansible.groups = {
      "Haproxy" => ["Haproxy"]

    }
    
  end
end
