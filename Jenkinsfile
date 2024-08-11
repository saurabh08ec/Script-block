pipeline {
    agent any
    stages {
        stage('Staging') {
            steps {
                echo 'Staging ....'
                script {
                    env.My_var = sh(script: 'date', returnStdout: true)
                }
            }
        }
        stage('E2E') {
            steps {
                echo 'E2E ....'
                echo "Today's date is ${env.My_var}"
            }
        }        
        stage('Deploy') {
            steps {
                echo 'Deploy ....'
                echo "Today's date is ${env.My_var}"
            }
        }        
    }
}
