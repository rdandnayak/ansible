# Ansible for Web Development [![Ansible workflow](https://github.com/rdandnayak/ansible/actions/workflows/manual.yml/badge.svg)](https://github.com/rdandnayak/ansible/actions/workflows/manual.yml)

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

you can clone this repository and run

```
./install
```

alternatively you can run below command to complete installation without pulling above repo
```
ansible-pull -U https://github.com/rdandnayak/ansible.git --skip-tags <ubuntu|macos> --ask-become-pass
```

which will take care of setting up your mentioned with tools mentioned above


Note:
this command will ask you for sudo password to do necessary insallations once
