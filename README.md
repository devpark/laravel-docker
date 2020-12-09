# Docker Start Up

### Prerequisites:

Working with docker environment requires installation below tools on workstation 
1. docker
2. docker-compose
3. composer

## Starting new project

### Install framework

1. New project starts with framework cloning
`git clone https://github.com/laravel/laravel.git`

2. Remove git history
`rm -rf .git`

3. Reinitial repository
`git init`

4. Add first commit
`git add . && git commit -m 'init'` 

5. Add remote repository.
`git remote add https://remote.repository.git`

6. Push initial commit to remote repository
`git push origin master`

### Adding docker enviroment

1. Download ZIP version of this repository.

2. Extract ZIP and put docker directory to project.

3. Move to docker directory in project
`cd /path/to/project/docker`  

4.  Build docker environment
`docker-compose build`

5. Up and running docker environment
`docker-composer up -d`

6. Visit welcome page laravel.docker (127.17.0.1) 

## Working with existing project

1. Clone project repository to local workstation
`git clone https://remote.repository.git`

2. Move to project directory
`cd /path/to/project` 

3. Switch to develop branch if existing
`git checkout develop` 

4. Move to docker directory in project
`cd /path/to/project/docker`  

5.  Build docker environment
`docker-compose build`

6. Up and running docker environment
`docker-composer up -d`


