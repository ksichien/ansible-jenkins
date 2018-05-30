Vagrant.configure(2) do |config|
  config.vm.box = 'debian/stretch64'
  config.vm.network 'private_network', ip: '10.20.20.20'
  config.vm.provider 'virtualbox' do |vb|
    vb.memory = '2048'
  end
  config.vm.provision 'ansible' do |ansible|
    ansible.playbook = 'vagrant.yml'
    ansible.inventory_path = 'hosts'
    ansible.verbose = '-v'
  end
end
