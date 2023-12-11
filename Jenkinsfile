pipieline{
  agent any
  stages {
    stage('Checkout'){
      steps {
        checkout([$class: 'GitSCM', branches: [[name: '*/main']], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'RelativeTargetDirectory', relativeTargetDir: 'your-web-app']], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/yourusername/your-web-app.git']]])
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
