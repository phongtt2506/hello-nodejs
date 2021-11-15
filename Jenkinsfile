pipeline{
  agent any
  stages{
    stage('Clone'){
      steps{
            git credentialsId: 'github', url: 'https://github.com/phongtt2506/hello-nodejs.git'
      //    echo "Hello world"
      }
    }
    stage('Build'){
      steps{
        withDockerRegistry(credentialsId: 'docker-hub', url: 'https://index.docker.io/v1/') {
          sh 'docker build -t phongtt2506/nodejs-test:v10 .'
          sh 'docker push -t phongtt2506/nodejs-test:v10 .'
        }
      }
    }
  }
}
