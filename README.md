# Weather App - DataOps

## Description

This is a weather forecasting app.

## Installation

- clone this repo 
- on your terminal
    - `cd` to root  folder
    - delete data folder to start your own
    - setup `.env` with:
        - `PORT` of your choosing
        - `CITY` of your choice
        - `API_KEY` from openweather
    - `npm i` to install dependencies 
    - `node fetchweather.js` to create/update data folder
    - `node app.js` to start server
- open browser on `PORT` to see weather and graph

## Using Docker

- Open your Docker Desktop
- Make sure you are on the same path as DockerFile
- On your terminal run:
    - `docker build -t <app-name>:<tag> .` or `docker build -t weatherappjs:1.0 .` - to build an image based on docker file
    - `docker run -p <local-port>:<container-port> <image-name>` or `docker run -p 3000:5000 weatherappjs`- to run a container based on an image

## Tests

We have tests to check if files inside the data folder is correct.