# Introduction 
Use the following steps to get the genesis environment up and running

# Requirements
Docker installed and daemon running

# Getting Started
Open a terminal and ssh into host device
`ssh user@ip`
OR 
On windows, use a program such as putty to login via ssh

download compose script
`curl -LJO https://raw.githubusercontent.com/tulsasoftware/ucontrol-genesis-compose/main/docker-compose.yml`
download template env variable
`curl -LJO https://raw.githubusercontent.com/tulsasoftware/ucontrol-genesis-compose/main/.env.template` 
create a production env from template
`mv .env.template .env`
edit your .env files, updating tokens, usernames, passwords, etc as needed
`nano .env`
run the genesis stack in the background
`docker-compose up -d`