from ubuntu:14.04

run apt-get update && apt-get install git curl wget build-essential -y
run wget -qO- https://deb.nodesource.com/setup_12.x | sudo -E bash -
run apt install -y nodejs
run curl -sL https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
run echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
run apt-get update && apt-get install yarn
run yarn global add @vue/cli@latest && yarn global add @vue/cli-service