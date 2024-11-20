pipline {
agent any

environment{
DOCKER_IMAGE = "ayoubhammou/myrepo:monitorinatag"
}

stages{
    stage('checkout git repo'){
        steps{
        git branch: 'main', url: 'https://github.com/Ayoub-HM/myrepo.git'

        }
    }

    stage('build docker image'){
        script{
        docker.build(DOCKER_IMAGE)
        }
    }
}
}
