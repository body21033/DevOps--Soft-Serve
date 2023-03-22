# HomeTask_01 - Vagrant (Installing VirtualBox)


## Requirements:
 - We need to have a Windows OS with PowerShell;
 - Install a hypervisor (`VirtualBox`);
 - Install `Vagrant`;
 - Using Vagrant creates virtual machine with OS Linux Ubuntu 20.04;
 - Provide your Vagrantfile and screenshot that demonstrates started VM;
 
## Preparation:
 - First you need to download [`VirtualBox`][1];
 - Second you should to install [`Vagrant`][2] with terminal;
 ___
 Some useful commands:
 - `sudo usermod -aG docker $USER`
 - `sudo usermod -aG sudo sammy` -- add permissions for user-sammy
 - `sudo useradd -m new-user` -- add new user with home-dir
 - `sudo pgrep -u old-user` -- stop all procceses from old-user
 - `sudo userdel -f old-user` -- remove user
  
## My results:

- If you want to check my servers, follow next links:
  
1. After installing `VirtualBox`- will install `Vagrant`:

![image](https://github.com/body21033/DevOps--Soft-Serve/blob/main/Lab_01/img/10.jpg?raw=true)

___

2. Let's run commands:
     - `vagrant box add centos/7` и выберем вариант 3 (VirtualBox);
     - `vagrant init centos/7`;
     - `vagrant up`:

![image](https://github.com/body21033/DevOps--Soft-Serve/blob/main/Lab_01/img/11.jpg?raw=true)

###

3. As a result, we started a virtual machine with the image `centos/7`.

___

1. Now let's start the virtual machine with custom settings:
     - vagrant box add ubuntu/focal64:
     
![image](https://github.com/body21033/DevOps--Soft-Serve/blob/main/Lab_01/img/3.jpg?raw=true)

     - vagrant init ubuntu/focal64:
![image](https://github.com/body21033/DevOps--Soft-Serve/blob/main/Lab_01/img/2.jpg?raw=true)

2. You should change the code in the `Vagrantfile` to the following:
          
    ## [`Vagrantfile`][4]
   - This can be done using a Notepad++
 ![image](https://github.com/body21033/DevOps--Soft-Serve/blob/main/Lab_01/img/12.jpg?raw=true)  
     
3. Visual code example [`Vagrantfile`][4]: 

 ![image](https://github.com/body21033/DevOps--Soft-Serve/blob/main/Lab_01/img/13.jpg?raw=true)

###

4. Execute the command `vagrant up`:

 ![image](https://github.com/body21033/DevOps--Soft-Serve/blob/main/Lab_01/img/4.jpg?raw=true)
 
 ###
 
5. Execute the command `vagrant ssh` and connect to our virtual machine:
 ![image](https://github.com/body21033/DevOps--Soft-Serve/blob/main/Lab_01/img/5.jpg?raw=true)
 
6. ### As we can see: the virtual machine is successfully configured)

___

## Useful Links:

1) [YouTube Channel for installing Vagrant][3]
2) [Ubuntu-images][5]
3) [Vagrant documentation][6]

[1]: https://www.virtualbox.org/wiki/Downloads
[2]: https://www.vagrantup.com/Downloads
[3]: https://youtu.be/8TJYZLe7vEc
[4]: https://github.com/body21033/DevOps--Soft-Serve/blob/8c3624221ed6540a9bafd0bce9532dbf9c4d429d/Lab_01/Vagrantfile
[5]: https://app.vagrantup.com/ubuntu
[6]: https://help.ubuntu.ru/wiki/vagrant
