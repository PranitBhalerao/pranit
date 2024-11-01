pipeline {
  agent any

  stages {
    stage('01.Clone Repo') {
      steps {
        git branch: 'main', credentialsId: 'Proj', url: 'git@github.com:PranitBhalerao/pranit.git'
      }
    }
    stage('01.Clean') {
      steps {
        bat 'mvn clean'
      }
    }
  }
}
