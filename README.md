# dockerfiles-windows
Various Dockerfiles for Windows. You probably have heard about Docker and that everyone uses Linux Containers. You can do this on Windows as well today with the Windows Server 2016 TP5 using Windows Containers.

## Getting started

* Register to [evaluate Windows Server 2016 TP5](https://technet.microsoft.com/de-de/evalcenter/dn781243.aspx).
* Get a Windows Server 2016 TP4/TP5 Virtual Machine
  * **Packer and Vagrant**
    * Use Packer with this [packer-windows](https://github.com/StefanScherer/packer-windows) templates to [build the ` windows_2016_tp5_docker` Vagrant box](https://github.com/StefanScherer/docker-windows-box#get-the-base-box).
    * Use Vagrant and this  [docker-windows-box](https://github.com/StefanScherer/docker-windows-box) Vagrantfile to have Docker and lots of Docker Tools installed.
  * **Azure**
    * Deploy TP4 VM to Azure with [`docker-windows-azure`](https://github.com/StefanScherer/docker-windows-azure) template
    * Create a [Windows Server 2016 Core with Containers TP4](http://azure.microsoft.com/en/marketplace/partners/Microsoft/WindowsServer2016TechnicalPreviewwithContainers/) Virtual Machine
  * Physical Machine / Virtual Machine
    * Read [Preparing a physical machine or an existing virtual machine for Windows Server Containers](https://msdn.microsoft.com/virtualization/windowscontainers/quick_start/inplace_setup) to install Docker into Windows 2016 TP4.
* Clone this repo and create some Docker images

## Further reading
  * Read the [Quick Start: Windows Server Containers and Docker](https://msdn.microsoft.com/virtualization/windowscontainers/quick_start/manage_docker) to get started with a first tutorial.
  * Read my blog post [Create a Node.js Container image for Windows](https://stefanscherer.github.io/create-an-io-js-container-image-for-windows/) for my first test drive with Docker on Windows.
  * Image what will happen when [Kitematic meets Windows Containers](http://blog.hypriot.com/post/kitematic-meets-windows-docker/).
  * **More Dockerfiles for Windows:** [Buc Rogers: Dockerfiles-for-Windows](https://github.com/brogersyh/Dockerfiles-for-windows)
  * **Windows Server Containers Examples**: https://github.com/Microsoft/Virtualization-Documentation/tree/master/windows-container-samples/windowsservercore

## PowerShell tricks
Porting Dockerfiles from Linux to Windows I found it useful to use PowerShell at some points. Here are some [PowerShell tricks](PowerShellTricks.md) that were useful for me.

## Feedback and Pull Requests are welcome
If you have some improvements, bug fixes, some new Dockerfiles or more PowerShell tricks, just send me a PR. If you have questions or problems, open an issue for discussion.

## License

MIT - for more details see the [LICENSE](./LICENSE) file.
