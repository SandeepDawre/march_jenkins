pipeline {
    agent any
    environment {
        F_NAME = 'TEST'
        L_NAME = 'USER'
     } 
    parameters {
        string(name: 'F_NAME02', defaultValue: 'HELLO', description: 'What is Your F Name .. ?')
        string(name: 'L_NAME02', defaultValue: 'MOTO', description: 'What is Your L NAME .. ?')
    }
    stages {
        stage('Stage 01') { 
            when {
                branch 'main'
            }            
            steps {
              echo "Hello I am from ${env.F_NAME} ${env.L_NAME}"
            }
        }
         stage('Stage 02') {
            when {
                branch 'master'
            }
            steps {
                echo "Hello I am from ${params.F_NAME02} ${params.L_NAME02}"

            }
        }
    }
}
