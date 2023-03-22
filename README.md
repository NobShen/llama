llama installation on ubuntu
>sudo apt update
>sudo apt upgrade
>sudo apt install build-essential python3-venv
>sudo apt install curl
>curl -sL https://deb.nodesource.com/setup_18.x -o nodesource_setup.sh
>sudo bash nodesource_setup.sh
use aptitude to avoid running into conflict with dpkg
>sudo apt install aptitude
>sudo aptitude install -y nodejs
verify node -v
now install alcapa 7B model
>npx dalai alcapa install 7B
or llama 7B model
>npx dalai llama install 7B

dd
