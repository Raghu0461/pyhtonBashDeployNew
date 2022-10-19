pipeline{
    agent any
    
    options {
       buildDiscarder(logRotator(numToKeepStr: '10'))
    }

    stages{
        
        stage('Message'){
            steps {
             echo "This Is Raghu Ram"
            }
        }
        stage('Python Script'){
             steps {
             sh 'program.py'
             }
        }
        stage('Bash Script'){
             steps {
             sh 'bashprogram.sh'
             }
        }
    }
}
