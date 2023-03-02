# To check if your APT mirror works and is serving packages correctly on your system, follow these steps:

1)Open a terminal window on your system.

2)Update the package lists: Type the following command and press Enter:

Copy code:-
```
sudo apt update
#This command updates the package lists from all the APT sources configured on your system.
```
3)Install a package: Type the following command and press Enter:

Copy code:-
```
sudo apt install <package-name>
#Replace <package-name> with the name of a package available in your APT mirror. 
```
For example, you can try installing the nginx web server package:

Copy code:-
```
sudo apt install nginx
#This command installs the specified package and any dependencies from your APT mirror.
```
4)Verify the installation: Once the package installation completes, you can verify that the package was installed from your APT mirror by running the following command:

Copy code:-
```
apt-cache policy <package-name>
#Replace <package-name> with the name of the package you just installed. This command shows the available versions of the specified package and their origin (i.e. which APT source they were downloaded from).
```
If the output shows that the package was downloaded from your APT mirror, then your mirror is working correctly.

By following these steps, you can verify that your APT mirror is serving packages correctly on your system.
