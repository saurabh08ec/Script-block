pipeline {
    agent any
    stages {
        stage('Staging') {
            steps {
                echo 'Staging ....'
                script {
                    env.My_var = "saurabh"
                    env.My_var1 = "Dubey"
                }
            }
        }
        stage('E2E') {
            steps {
                echo 'E2E ....'
                echo "My name is ${env.My_var}"
            }
        }        
        stage('Deploy') {
            steps {
                echo 'Deploy ....'
                echo "My name is ${env.My_var} ${env.My_var1}"
            }
        }        
    }
}
