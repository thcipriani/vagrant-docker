# TO RUN THIS FILE:
# sudo docker pull ubuntu
# sudo vagrant up --provider=docker

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.synced_folder "./www", "/var/www"

  config.vm.provider "docker" do |d|
    d.build_dir = "./Docker"
    d.ports << '80:80'
  end
end
