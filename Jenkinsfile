pipeline{
    agent any
    
    options {
       buildDiscarder(logRotator(numToKeepStr: '10'))
    }

    stages{
        
        stage('GIT CHECKOUT'){
            steps {
            git branch: 'main', url: 'git@github.com:Raghu0461/pyhtonBashDeployNew.git'
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
