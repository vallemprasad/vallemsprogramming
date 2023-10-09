pipeline {
  agent any
  stages {
    stage("build") {
        steps{
    echo 'Baba is building the application...'
        }
    }
    stage("Test") {
        steps {
    echo 'Baba is testing the application...'
        }
    }
    stage("deploy") {
      steps {
    echo 'Baba is deploying the application...'
    sh 'python3 hello.py'
      }
    }
  }
}
