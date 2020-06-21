#!groovy

node('ecs-agent') {
    git 'https://github.com/MikhailZheltyshev/users-api.git'
    def newApp = docker.build "mihalichzh/usersapi:latest"
    newApp.push()
}