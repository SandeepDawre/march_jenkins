pipeline {
    agent any
    environment {
        F_NAME = 'TEST'
        L_NAME = 'USER'
     } 
    parameters {
        string(name: 'F_NAME02', defaultValue: 'F_NAME02', description: 'What is F_NAME02 .. ?')
        string(name: 'L_NAME02', defaultValue: 'L_NAME02', description: 'What is L_NAME02 .. ?')



        //string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
        //text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')
        //booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')
        //choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')
        //password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')

    }
    stages {
//THIS STAGE NO 1
        stage('Echo Stage') { 
            steps {
              echo "Hello I am from ${env.F_NAME} ${env.L_NAME}"
            }
        }
//THIS STAGE NO 2
         stage('Example') {
            steps {
                echo "Hello I am from ${params.F_NAME02} ${params.L_NAME02}"
                echo "Hello my hostname is ${env.HOSTNAME}"
                //echo "Hello ${params.PERSON}"
                //echo "Biography: ${params.BIOGRAPHY}"
                //echo "Toggle: ${params.TOGGLE}"
                //echo "Choice: ${params.CHOICE}"
                //echo "Password: ${params.PASSWORD}"
            }
        }
    }
}
