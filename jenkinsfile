pipeline {
  agent any

  stages {
    stage ("Docker image") {
      steps {
        dockerapp = docker.build("fabricioveronez/kube-news:${env.BUILD_ID}", "-f ./src/Dockerfile ./src")
      }
    }
  }
}

