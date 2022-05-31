# TicTacToe Remake

## Project description

A simple Django web implementation of a classic game Tic Tac Toe, to showcase the use of:

* Docker - a software framework for containerizing applications
  
* Django - a Python web framework
  
* Modern and minimal game architecture - FSM powered
  
* Game AI Agent - powered by Minimax and Alpha-beta pruning algorithms

## Docker setup

A simple docker setup utilizing python:3 image and docker-compose as the building driver.

Although docker-compose is recommended as a tool for managing multiple containers, it's used in this project with the ease-of-use and with future expansion in mind.

Run initial compose with:

```console
user@host:~$ sudo docker-compose run web django-admin startproject TicTacToeRemake .
```

(Only on Linux) Change owner for files created with Django:

```console
user@host:~$ sudo chown -R $USER:$USER TicTacToeRemake manage.py
```

Compose up to run the app:

```console
user@host:~$ sudo docker-compose up
```

## TODOs

* [ ] Refactor the old app
* [ ] Make Django web view for the app
* [ ] Recheck the AI algorithms
