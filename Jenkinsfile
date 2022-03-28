pipeline {
    agent any

    stages {
        stage('unit test ') {
            steps {
                echo 'Hello to everyone'
            }
    }
            stage('build ') {
            steps {
                echo 'Hello to everyone'
       
            }
    }        
            stage('Deploy ') {
                input {
                    message 'shell we deploy to production'
                    ok "yes we may proceed"
                }

            steps {
                echo 'Hello to everyone'
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
