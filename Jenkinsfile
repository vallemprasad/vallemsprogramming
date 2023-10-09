pipeline {
  agent any
  environment {
    PYTHON_PATH = "/usr/bin/python3"
    }
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
        }
    }
  }
}
