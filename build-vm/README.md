How to create your own virtual machine using scripts ? 

1. download and install Oracle Virtual Box on your machine. 
2. download and install vagrant on your machine . 
3. download the vagrant file given and store it in the location you want the virtual machine . 
4. navigate to this location via cmd(windows) or terminal (ubuntu) and give command vagrant up . 

Acknowledgements : 
1. how to configure the virtual box using vagrant has been taken from here: (https://docs.vagrantup.com/v2/virtualbox/configuration.html)
2. how to install java has been taken from here: 
   (https://github.com/aglover/ubuntu-equip)

#Steps to create Virtual Machine using Vagrant
1. Download and Install [Virtual Box](https://www.virtualbox.org/wiki/Downloads) on the host machine.
2. Download and Install [Vagrant](https://www.vagrantup.com/downloads.html) on the host machine.
3. Create a new directory on your machine and download this [Vagrantfile](https://github.com/SoftwareEngineeringToolDemos/ICSE-2014-Viva/blob/master/build-vm/Vagrantfile) into that directory.
4. Navigate to the directory and run the command: "vagrant up". This command downloads the VM box for the VirtualBox provider (if the box is not already present). It then spins up the VM, which is a 64-bit Ubuntu 14.04 Desktop Edition VM with Java 8 installed in it. The "--provision" option installs additional software on the VM, which can be specified in the Vagrantfile.
5. To restart the VM, run the command: "vagrant reload". 
6. To shutdown the VM, run the command: "vagrant halt" if you want vagrant to attempt a graceful shutdown. If not, then run the command: "vagrant halt -f"

#Note
* Please wait until "vagrant up" command has completed successfully before using the virtual machine.
* VM login details if required:</br>
User     : vagrant</br>
Password : vagrant 

* Run the command:
~~~
java -version
~~~
 to verify the installation of JDK 8 on the VM. You should expect to see an output similar to this:
~~~
java version "1.8.0_66"
Java(TM) SE Runtime Environment (build 1.8.0_66-b17)
Java HotSpot(TM) 64-Bit Server VM (build 25.66-b17, mixed mode)
~~~
# Acknowledgments
* Used vagrant virtual box image of [ubuntu-trusty64-gui by chad-thompson](https://atlas.hashicorp.com/chad-thompson/boxes/ubuntu-trusty64-gui).

#References
* https://docs.vagrantup.com/v2/getting-started/index.html
* https://docs.vagrantup.com/v2/provisioning/shell.html 
* https://docs.vagrantup.com/v2/virtualbox/configuration.html
* https://github.com/aglover/ubuntu-equip


