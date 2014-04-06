Vagrant.require_version '>= 1.6'

Vagrant.configure('2') do |config|
  config.vm.box = 'hashicorp/precise64'
  config.vm.provision :shell, :path => "bootstrap.sh"

  # flavorjones added
  config.vm.synced_folder "/home/miked-public/code/oss",            "/home/vagrant/oss"
  config.vm.synced_folder "/home/miked-public/Shared/Virtualboxen", "/home/vagrant/shared"
  config.vm.provider "virtualbox" do |v|
    v.memory = 1024
    v.cpus = 2
  end
end
