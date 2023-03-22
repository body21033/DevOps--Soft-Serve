# HomeTask_01 - Vagrant (Installing VirtualBox)


## Requirements:
 - We need to have a Linux OS;
 - Install a hypervisor (VirtualBox)
 - Install Vagrant
 - Using Vagrant create virtual machine with OS Linux Ubuntu 20.04
 - Provide your Vagrantfile and screenshot that demonstrates started VM
 
## Preparation:
 - First you need to download [`VirtualBox`][1];
 - Second you should to install [`Vagrant`][2] with terminal;
  
## My results:

- If you want to check my servers, follow next links:
  
1. After installing `VirtualBox`- will install `Vagrant`:

![image](https://github.com/body21033/DevOps--Soft-Serve/blob/main/Lab_01/img/10.jpg?raw=true)

2. Запустим команды:
     - `vagrant box add centos/7` и выберем вариант 3 (VirtualBox);
     - `vagrant init centos/7`;
     - `vagrant up`:

![image](https://github.com/body21033/DevOps--Soft-Serve/blob/main/Lab_01/img/11.jpg?raw=true)

3. В результате у нас запустилась виртуальна машина с образом `centos/7`.

1. Теперь запустим виртуальную машину с пользовательскими настройками:
     - vagrant box add ubuntu/focal64:
     
![image](https://github.com/body21033/DevOps--Soft-Serve/blob/main/Lab_01/img/3.jpg?raw=true)

     - vagrant init ubuntu/focal64:
![image](https://github.com/body21033/DevOps--Soft-Serve/blob/main/Lab_01/img/2.jpg?raw=true)

2. Следует изменить код в файле `Vagrantfile` на следующий:
          
    ## [`Vagrantfile`][4]
   - Это можно сделать при помощи Notepad++
 ![image](https://github.com/body21033/DevOps--Soft-Serve/blob/main/Lab_01/img/12.jpg?raw=true)  
     
3. Визуальный пример кода `Vagrantfile`: 
 ![image](https://github.com/body21033/DevOps--Soft-Serve/blob/main/Lab_01/img/13.jpg?raw=true)

4. Выполняем команду `vagrant up`:
 ![image](https://github.com/body21033/DevOps--Soft-Serve/blob/main/Lab_01/img/4.jpg?raw=true)
 
5. Выполняем команду `vagrant ssh` и подключаемся к нашей виртуальной машине:
 ![image](https://github.com/body21033/DevOps--Soft-Serve/blob/main/Lab_01/img/5.jpg?raw=true)

## Useful Links:

1) [YouTube Channel for installing Vagrant][3]

[1]: https://www.virtualbox.org/wiki/Downloads
[2]: https://www.vagrantup.com/Downloads
[3]: https://youtu.be/8TJYZLe7vEc
[4]: https://github.com/body21033/DevOps--Soft-Serve/blob/8c3624221ed6540a9bafd0bce9532dbf9c4d429d/Lab_01/Vagrantfile
