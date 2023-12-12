pipeline{
  agent any
  stages {
    stage('Checkout'){
      steps {
         checkout([$class: 'GitSCM', branches: [[name: '*/main']], doGenerateSubmoduleConfigurations: false, userRemoteConfigs: [[url: 'https://github.com/harshada-zurunge/Web-Application.git']]])
      }
    }
    stage('Build'){
      steps{
        echo 'Building'
      }
    }
    stage('Deploy'){
      steps{
        echo 'Deploying'
      }
    }
  }
}



