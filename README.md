# wain-meanstack
This is a Mean stack Wain dashboard.

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/93ce59cb56fe34e4cb7f)

### Install Dependencies
* [Vagrant](https://www.vagrantup.com/downloads.html)
* [Virtualbox](https://www.virtualbox.org/wiki/Downloads)
* After the instalation of Vagrant and Virtualbox
```bash
   vagrant up
   npm install webpack -g
   cd admin/public
   npm install
```

### Setup Front-End for Development
```bash
   cd admin/public
   webpack --watch
```
### Run
```bash
   vagrant ssh
   cd /vagrant
   npm i --no-bin-links
   npm start
```
### Logout
```bash
   logout
   vagrant halt
```
### Update Back-end Server
```bash
   cd /usr/share/nginx/wain-meanstack
   forever list
   kill [pid]
   git pull
```