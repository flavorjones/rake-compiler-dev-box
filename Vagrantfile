Vagrant.require_version '>= 1.6'

Vagrant.configure('2') do |config|
  config.vm.box = 'hashicorp/precise64'
  config.vm.provision :shell, :path => "bootstrap.sh"

  # flavorjones added
  config.vm.synced_folder "/home/flavorjones/code/oss",            "/home/vagrant/oss"
  config.vm.synced_folder "/home/flavorjones/Shared/Virtualboxen", "/home/vagrant/shared"
  config.vm.provider "virtualbox" do |v|
    v.memory = 1024
    v.cpus = 3
  end
end
