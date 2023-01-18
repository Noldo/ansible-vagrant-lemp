Vagrant.configure("2") do |config|

  config.vm.box = "generic/ubuntu2204"

  config.vm.network "private_network", ip: "192.168.33.23"

  config.vm.synced_folder "../html", "/var/www/html"
  config.vm.define "php-react"

  config.vm.provision "ansible" do |ansible|
    ansible.verbose = "v"
    ansible.playbook = "provisioning/playbook.yml"
  end
end
