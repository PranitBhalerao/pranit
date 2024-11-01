pipeline {
  agent any

  stages {
    stage('01.Clone Repo') {
      steps {
        echo "cloned"
        //git branch: 'main', credentialsId: 'Proj', url: 'git@github.com:PranitBhalerao/pranit.git'
      }
    }
    stage('02.Clean') {
      steps {
        echo "cleaning"
         //bat 'mvn clean'
      }
    }
    stage('03.Package') {
      steps {
        bat 'mvn package'
      }
    }
  }
}
