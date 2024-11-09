pipeline {
  agent any

  stages {
    stage('01.Clone Repo') {
      steps {
       git branch: 'main', credentialsId: 'Proj', url: 'git@github.com:PranitBhalerao/pranit.git'
      }
    }
    stage('02.Clean') {
      steps {
        bat 'cd pranit && mvn clean'
      }
    }
    stage('03.Package') {
      steps {
       bat 'cd pranit && mvn package'
      }
    }
  }
}
