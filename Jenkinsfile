pipline {
agent any

environment{
DOCKER_IMAGE = "ayoubhammou/myrepo:monitorinapp2"
}

stages{
    stage('checkout git repo'){
        steps{
        git 'https://github.com/Ayoub-HM/myrepo/tree/main/Monitoring'

        }
    }

    stage('build docker image'){
        script{
        docker.build(DOCKER_IMAGE)
        }
    }
}
}