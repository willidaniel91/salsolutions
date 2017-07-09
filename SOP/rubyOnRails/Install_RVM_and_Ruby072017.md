#### Ruby Version Manager and Ruby

---
#### Installation Guide

1. To install RVM, type this in your terminal:
```
\curl -L https://get.rvm.io | bash -s stable
```
2. Close your terminal and then re-open it. Now, lets see if RVM was loaded properly:
```
rvm | head -n 1
```
3. Now install Ruby with:
```
rvm use ruby --install --default
```
* this will set the installed version of ruby as the default version to be used.
4. Check for the version of Ruby:
`ruby -v`

5. *List all versions of Ruby on system:
```
rvm List
```
6. change version of Ruby to version 2.1.1:
```
rvm use 2.1.1
```
*or* to change the default version of Ruby:
```
rvm --default 2.1.1
```

[source](http://installrails.com/steps/install_rvm_and_ruby)

---
last edited and verified by Andrew Hunsaker on 7.7.2017
