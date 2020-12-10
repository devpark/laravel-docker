# Laravel Start Up

### Prerequisites:

Working with docker environment requires installation below tools on workstation 
1. docker
2. docker-compose
3. composer

## Starting new project

### Install framework

1. New project starts with framework cloning
`git clone https://github.com/laravel/laravel.git`

2. Go to project directory in project 
`cd /path/to/laravel/project`

2. Remove git history
`rm -rf .git`

3. Reinitial repository
`git init`

4. Add first commit
`git add . && git commit -m 'init'` 

5. Add remote repository.
`git remote add origin https://remote.repository.git`

6. Push initial commit to remote repository
`git push origin master`

### Adding docker environment

1. Download ZIP version of this repository.

2. Extract ZIP and put docker directory to project.

3. Fill  environment variables in `.env.example`

***Caution:\
Filling environment variables .env.example should pairing with docker compose configuration\
Use this repository sample .env.example***

## Working with existing project

1. Clone project repository to local workstation
`git clone https://remote.repository.git`

2. Move to project directory
`cd /path/to/project` 

3. Switch to develop branch if existing
`git checkout develop` 

4.  Make you own environment 
`cp .env.example .env`

***Caution:\
Sample environment variables .env.example should pairing with docker compose configuration\
Don't need to make any changes***  

5. Move to docker directory in project
`cd /path/to/project/docker`  

6.  Build docker environment
`docker-compose build`

7. Up and running docker environment
`docker-compose up -d`


## Startup Projects

1.  Make you own environment 
`cp .env.example .env`

2. Move to docker directory in project
`cd /path/to/project/docker`  

3.  Build docker environment
`docker-compose build`

4. Up and running docker environment
`docker-compose up -d`


## Install Laravel


1. Install dependencies
 
`docker exec -it ${project-name}-backend composer install`

***${project-name} is your project name, check by docker ps***

2. Generate api key
 
`docker exec -it ${project-name}-backend php artisan key:generate`

5. Visit welcome page laravel.docker (127.17.0.1) 
