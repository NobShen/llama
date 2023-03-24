llama installation on ubuntu
After installation, the system already has python3 v 3.10.6 installed
But you don't have nodejs installed yet
You can update & upgrade but I didn't
>sudo apt update
>sudo apt upgrade

Then install build tools to build dalai llama
>sudo apt install build-essential

Then download node version 18.x
>sudo apt install curl
>curl -sL https://deb.nodesource.com/setup_18.x -o nodesource_setup.sh
>sudo bash nodesource_setup.sh
use aptitude to avoid running into conflict with dpkg
>sudo apt install aptitude
>sudo aptitude install -y nodejs
verify node -v (v18.15.0)

now install llama 13B model
>npx dalai llama install 13B
>dalai@0.3.1 will be installed

now run it
> sudo npx dalai serve
Your server will run at localhost:3000

That's it!

