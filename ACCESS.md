# How others can access your APT mirror
1)Once you have set up your APT mirror and configured your web server, others can access your APT mirror by using the URL you have created for it.

For example, if you have set up your APT mirror with Nginx and your domain name is `yourdomain.com`, others can access your APT mirror by adding the following line to their `/etc/apt/sources.list` file:

Copy code:-
```
deb http://yourdomain.com/ubuntu focal main restricted universe multiverse
```
2)They can then run sudo apt-get update on their system to update their package lists and download packages from your APT mirror.

If you have set up your APT mirror with Apache2, they would add the following line to their `/etc/apt/sources.list` file:

Copy code:-
```
deb http://yourdomain.com/ubuntu focal main restricted universe multiverse
```
3)Again, they can then run `sudo apt-get update` to update their package lists and download packages from your APT mirror.

4)Make sure to provide the URL to the users who need to access your APT mirror.
