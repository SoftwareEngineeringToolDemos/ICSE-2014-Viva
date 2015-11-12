Vagrant.configure(2) do |config|
  config.vm.box = "boxcutter/ubuntu1404-desktop"
  config.vm.provider "virtualbox" do |vb|
       vb.gui = true
       vb.memory = "1024"
       vb.name="esharma2_Viva"
    end
  config.vm.provision "shell", inline: <<-SHELL
    sudo apt-get update
    wget --no-check-certificate https://github.com/aglover/ubuntu-equip/raw/master/equip_java8.sh && bash equip_java8.sh
   SHELL
end
