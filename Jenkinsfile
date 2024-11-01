pipeline {
  agent any

  stages {
    stage('Checkout') {
      steps {
        git branch: 'main', credentialsId: 'Proj', url: 'git@github.com:PranitBhalerao/pranit.git'
      }
    }
  }
}
