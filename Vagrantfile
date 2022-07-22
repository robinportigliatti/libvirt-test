Vagrant.configure("2") do |config|
  # Configuration du primary
  #config.ssh.private_key_path = "~/.ssh/id_rsa"
  config.ssh.forward_agent = true
  config.vm.define "host1" do |ovhneopbd1|
    ovhneopbd1.vm.box = "generic/ubuntu1804"
    ovhneopbd1.vm.hostname = "host1"
    ovhneopbd1.vm.network :private_network, ip: "192.168.60.11"
    ovhneopbd1.vm.provider :libvirt do |v|
      #v.gui = true
      v.cpus = 2
      v.memory = 1024
    end
  end
end # Vagrant.configure("2") do |config|
