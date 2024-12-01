pipeline {
  agent any

  stages {
    stage('01.Clone Repo') {
      steps {
       git branch: 'main', credentialsId: 'Bhale007', url: 'git@github.com:PranitBhalerao/pranit.git'
      }
    }
    stage('02.Clean') {
      steps {
        sh 'mvn clean'
      }
    }
    stage('03.Package') {
      steps {
       sh 'mvn package'
      }
    }
  }
}
