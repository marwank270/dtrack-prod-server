# Vagrant Installation


## Requirements
Vagrant require a virtualization product such as [VirtualBox](https://www.virtualbox.org/), [VMware Fusion](https://customerconnect.vmware.com/downloads/get-download?downloadGroup=FUS-PUBTP-2021H1), or [Hyper-V](https://docs.microsoft.com/en-us/virtualization/hyper-v-on-windows/quick-start/enable-hyper-v).
For the Production server I am using VirtualBox which also require [Microsoft Visual C++ 2019 Redistribuable](https://learn.microsoft.com/fr-fr/cpp/windows/latest-supported-vc-redist?view=msvc-170) on Windows.

After the installation of vc_2019, then VirtualBox we can download the appropriate version of [Vagrant](https://developer.hashicorp.com/vagrant/downloads).
## Initialization
After installation open a powershell window and run `vagrant --version` to make sure that [the latest release](https://github.com/hashicorp/vagrant/releases/latest) is installed.

A simple init command, thanks to [vagrant cloud](https://app.vagrantup.com/ubuntu/boxes/focal64) helps us having everything we need downloaded and installed.

```powershell
PS C:\Users\dev\vm> vagrant init ubuntu/focal64
PS C:\Users\dev\vm> vagrant up
```
Done, The Ubuntu is installed and up in background. To interact with it just connect to it with:
```powershell
PS C:\Users\dev\vm> vagrant ssh
```
On the first boot it will take some time to connect, because of the first initialisation of the vm.