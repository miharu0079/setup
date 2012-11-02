#Develop With Passion® - Presentation Setup

##The following setup should take between 20-30 minutes to complete depending on your skill level and familiarity with unix based environments.

##The two main programs you will need to install are:

* Ruby
* Git 


#Required Setup

The following is the setup that you WILL need to perform to configure all necessary prerequisites to be able to enjoy the week. If you have any questions, please do not hesitate to ask!!

##If you are running on windows - make sure that you have configured windows to show all hidden files and folders

##Get setup at [Github](http://github.com)

* [Sign up](https://github.com/signup/free) for a free account at github.com. My recommendation is to use an all lowercase username.

##Install Ruby

* Unix based OS

  * Install Ruby by using [rvm](https://rvm.io/rvm/install/)

* Windows based OS

  * Install the latest version of Ruby from [here](http://rubyforge.org/frs/download.php/76054/rubyinstaller-1.9.3-p194.exe)
  * Make sure you select the following options:
    * Add Ruby Executables to your path
    * Associate .rb and .rbw files with this Ruby installation
  * Once the install has completed, verify your installation by opening up a command prompt and typing in: ruby -v. You should see:
    * ruby 1.9.3 [version and date information]

##Install Git

* OSX
  * Install brew using the following instructions:
  ![brew install](http://github.com/camug2012nov/setup/raw/master/images/brew_install.png)
  * After brew is successfully installed, install git by typing the following command in a terminal window:
    * brew install git  

* Unix
  * Install git using the instructions outlined [here](http://git-scm.com/book/en/Getting-Started-Installing-Git)  

* Windows
  1. Install the latest version of Git for windows from [here](http://code.google.com/p/msysgit/downloads/detail?name=Git-1.7.11-preview20120710.exe&can=2&q=)

  * Configure according to the following screenshots:

  ![git_setup_part_1](http://github.com/camug2012nov/setup/raw/master/images/git_setup_part_1.png)
  ![git_setup_part_2](http://github.com/camug2012nov/setup/raw/master/images/git_setup_part_2.png)

##Setup your git ssh authentication key

1. Open up a git bash prompt
2. Enter the following command:    
   ssh-keygen -t rsa -C your_email_address  
   Accept the defaults for the remaining prompts  (leave the passphrase blank).  
3. Navigate to the folder where your ssh key was created (by default your profile folder)
4. Open the file id_rsa.pub and copy the contents to the clipboard.
5. Login to your account at [github](https://github.com/login).
6. Navigate to your [ssh settings](https://github.com/account/ssh)
7. Click on the link: Add Another Public Key:
8. Give your key a title and paste the public key that is in your clipboard from step 4 into the Key text entry:

![ssh key entry](http://github.com/camug2012nov/setup/raw/master/images/add_ssh_key.png)

##Verify that your git ssh authentication works

1. Open up a git bash prompt
2. Enter the following command:
   ssh -v git@github.com

3. You may be prompted to cache the server identity (type yes)
4. If you have setup your ssh settings correctly the bottom part of the command output should look similar to the following:

![successful authentication](http://github.com/camug2012nov/setup/raw/master/images/git_authentication.png)

##Clone this setup repository

1. Open up a shell (Terminal on osx, git bash on windows, or equivalent unix based shell) and type the following commands:
  * cd ~/ [enter]
  * mkdir camug_nov_2012 [enter]
  * cd camug_nov_2012 [enter]
  * git clone http://github.com/camug2012nov/setup.git [enter]

At the completion of the last command you should have a copy of this repository on your local machine.

##Update git and bash configuration details

The following steps will ensure that you have your git environment configured in the correct way for class. If you already have existing git configuration that you use on a regular basis, either make your changes manually to match the recommended settings, or create a backup of your existing configuration and restore it after the class.

Open up a shell (Terminal on osx, git bash on windows, or equivalent unix based shell) and type the following commands:

1. cd ~/camug2012nov/setup [enter]
2. ./copy_config [enter]
3. Edit the following file in your favourite editor: ~/.gitconfig 
    * change the email and name settings under the [user] section. Save your changes


##Fork the presentation repository

1. Login to your account at [github](https://github.com/login)
2. Search for the username camug2012nov: (Username in screenshot is for example purposes only)<br>![Search for camug2012nov](http://github.com/camug2012nov/setup/raw/master/images/github_search_for_develop_with_passion.png)
3. Click on the camug2012nov user (screenshot is for example purposes only)<br>![camug2012nov user](http://github.com/camug2012nov/setup/raw/master/images/github_developwithpassion_user.png)
4. Click on the code repository (screenshot is for example purposes only): ![repository](http://github.com/camug2012nov/setup/raw/master/images/github_shawaugp.png)
5. Click on the fork button to create your own copy of this repository <br>![fork](http://github.com/camug2012nov/setup/raw/master/images/github_fork.png)

## Checkout your local copies of the code

1. Open up a shell (Terminal on osx, git bash on windows, or equivalent unix based shell) and type the following commands:
  * cd ~/camug2012nov [enter]
  * git clone git@github.com:[your github user name]/code.git [enter]
    
    Assuming your github username is jp the command would look as follows:

    git clone git@github.com:jp/code.git [enter]
