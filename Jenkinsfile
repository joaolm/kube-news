pipeline {
  agent any

  stages {

    stage ('Build Docker Image') {
      steps {
        script {
          dockerapp = docker.build("joaolm/kube-news:${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
        }
      }
    }
  }
}