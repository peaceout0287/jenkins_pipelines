pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'echo "test"'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'hi'
          }
        }

        stage('deploy') {
          steps {
            echo 'deploy'
          }
        }

      }
    }

  }
}