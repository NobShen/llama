llama installation on ubuntu
After installation, the system already has python3 v 3.10.6 installed

>sudo apt update
>sudo apt upgrade
>sudo apt install build-essential
>No install of yet python3-venv
>sudo apt install curl
>curl -sL https://deb.nodesource.com/setup_18.x -o nodesource_setup.sh
>sudo bash nodesource_setup.sh
use aptitude to avoid running into conflict with dpkg
>sudo apt install aptitude
>sudo aptitude install -y nodejs
verify node -v (v18.15.0)

now install alcapa 7B model
>npx dalai alcapa install 13B
>dalai@0.3.1 will be installed
>
or llama 7B model
>npx dalai llama install 7B
To list all python versions in default locations

ls /usr/bin/python*

To remove just python3 package

sudo apt-get remove python3.5

plus it's dependent packages

sudo apt-get remove --auto-remove python3.5

plus configuration and/or data files of python3

sudo apt-get purge python3.5

both configuration and/or data files of python3.5 and it's dependencies

sudo apt-get purge --auto-remove python3.5

How to install new version of python

sudo apt-get update

sudo apt-get install python3

Also, see https://docs.python-guide.org/starting/install3/linux/ or install python3.8 https://linuxize.com/post/how-to-install-python-3-8-on-ubuntu-18-04/

ModuleNotFoundError: No module named '_sqlite3'.

sudo apt-get install libsqlite3-dev
./configure --enable-loadable-sqlite-extensions && make && sudo make install
