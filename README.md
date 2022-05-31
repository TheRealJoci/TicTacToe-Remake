# TicTacToe Remake

## Project description

A simple Django web implementation of a classic game Tic Tac Toe, to showcase the use of:

* Docker - a software framework for containerizing applications
  
* Django - a Python web framework
  
* Modern and minimal game architecture - powered by FSM logic
  
* Game AI Agent - powered by Minimax and Alpha-beta pruning algorithms

## Environment description

A simple docker setup utilizing python:3 image and docker-compose as the building driver.

Although docker-compose is recommended as a tool for managing multiple containers, it's used in this project for the ease of setup and with future expansion in mind.

## TODOs

* [x] Containerize the app with Docker
  * [x] Make a Dockerfile
  * [x] Make a docker-compose file
* [ ] Make a Django web app
  * [x] Make the "game" app
  * [ ] Make templates
  * [ ] Make views
* [ ] Refactor the old app
  * [ ] Rebuild the game logic to use reducer for driving the FSM
  * [ ] Recheck the AI algorithms
