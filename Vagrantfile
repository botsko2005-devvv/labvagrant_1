Vagrant.configure("2") do |config|
  # Перша віртуальна машина — Ubuntu 24.04 LTS (більше ресурсів)
  config.vm.define "ubuntu" do |ubuntu|
    ubuntu.vm.box = "bento/ubuntu-24.04"
    ubuntu.vm.hostname = "ubuntu-node"

    ubuntu.vm.provider "virtualbox" do |vb|
      vb.name = "Lab1_Ubuntu_24.04"
      vb.memory = "2048"
      vb.cpus = 2
    end
  end

  # Друга віртуальна машина — Debian 12 (менше ресурсів)
  config.vm.define "debian" do |debian|
    debian.vm.box = "bento/debian-12"
    debian.vm.hostname = "debian-node"

    debian.vm.provider "virtualbox" do |vb|
      vb.name = "Lab1_Debian_12"
      vb.memory = "1024"
      vb.cpus = 1
    end
  end
end