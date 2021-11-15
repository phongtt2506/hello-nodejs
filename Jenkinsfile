pipeline{
  agent any
  stages{
    stage('Clone'){
      steps{
        git 'https://github.com/phongtt2506/hello-nodejs.git'
      }
    }
    stage('Clone'){
      steps{
        withDockerRegistry(credentialsId: 'docker-hub', url: 'https://index.docker.io/v1/') {

        }
      }
    }
  }
}
