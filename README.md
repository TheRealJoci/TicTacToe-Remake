# TicTacToe Remake

## Project description

A simple Django web implementation of a classic game Tic Tac Toe, to showcase the use of:

* Docker - a software framework for containerizing applications
  
* Django - a Python web framework
  
* Modern and minimal game architecture - FSM powered
  
* Game AI Agent - powered by Minimax and Alpha-beta pruning algorithms

## Environment setup

A simple docker setup utilizing python:3 image and docker-compose as the building driver.

Although docker-compose is recommended as a tool for managing multiple containers, it's used in this project for the ease of setup and with future expansion in mind.

**REMINDER**

After any changes to the project requirements rebuild the service:

```console
user@host:~$ sudo docker-compose build --no-cache [SERVICE...]
```

## TODOs

* [ ] Refactor the old app
* [ ] Make TicTacToe Django app
* [ ] Recheck the AI algorithms
