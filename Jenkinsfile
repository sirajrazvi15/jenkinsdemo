pipeline {
  agent any
  stages {
    stage('unit test ') {
      parallel {
        stage('unit test ') {
          steps {
            echo 'Hello to everyone'
          }
        }

        stage('test2') {
          steps {
            sh 'echo "hello devops engineer"'
          }
        }

      }
    }

    stage('build ') {
      parallel {
        stage('build ') {
          steps {
            echo 'Hello to everyone'
          }
        }

        stage('build2') {
          steps {
            sleep 50
          }
        }

      }
    }

    stage('Deploy ') {
      parallel {
        stage('Deploy ') {
          input {
            message 'shell we deploy to production'
            id 'yes we may proceed'
          }
          steps {
            echo 'Hello to everyone'
          }
        }

        stage('deploy2') {
          steps {
            retry(count: 50) {
              sleep 10
            }

          }
        }

      }
    }

    stage('deploytoprod ') {
      steps {
        echo 'Hello to everyone'
      }
    }

  }
  post {
    always {
      echo 'always run the project'
    }

    failure {
      echo 'fail and run'
    }

  }
}