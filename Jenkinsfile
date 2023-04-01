pipeline {
    agent any
    environment {
        F_NAME = 'TEST'
        L_NAME = 'USER'
     } 
    stages {
        stage('Echo Stage') { 
            steps {
              echo "Hello I am from ${env.F_NAME} ${env.L_NAME}"
            }
        }
    }
}
