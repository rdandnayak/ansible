# Ansible for Web Development

This is Ansible repository which can be used to bring your machine up-to-speed by installing all necessary tools required to develop Web applications

## Installtions by Ansible

This will install following tools on your machine
1. zsh terminal with custom configuration
2. various npm packages
    1. yarn
    2. eslint
    3. typescript-language-server
    4. typescript
    5. ts-node
3. node version 14
4. vim & neovim code editor
5. necessary dotfiles required and mentioned in repo [link to .dotfiles repository](https://github.com/rdandnayak/.dotfiles)

## setup & installation for WSL or Ubuntu

if you are on Linux terminal or WSL

you can simply clone this repository and run

```
./ansible-install
```

which will take care of installing ansible on your machine,
```
ansible-playbook local.yml --ask-become-pass
```
above package will help you setting up your machine with required packages as mentioned above
above command will ask your user password once during installation

## setup and installation with docker

If you have docker demon & cli setup on your machine you can simply use command below to build brand new docker environment to start experimenting around ansible

1. Use command below
```
./build-dockers
```

2. Use command below to run ansible inside docker environment
```
./run-dockers
```

this will bring up docker container that will be ready to execute commands

run command below to run ansible inside your docker interactive terminal

```
ansible-playbook local.yml
```

which will run all necessary packages in mentioned list above, inside container
