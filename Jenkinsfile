pipeline {
    agent any
    stages {
        stage('Hello') {
            steps{
                script{
                  output= multiply()
                  echo "The multiplication result is ${output}"
            }
            }
        }
    }
}

def multiply()
    {
       def a=2
       def b=3
       def result=a*b
       return result
    }
