pipeline {
    agent any
        
    
    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage('Build') {
            steps {
                echo "construindo.."
                sh '''
                cd comandos
                pip install -r requisitos.txt
                '''
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
                sh '''
                cd constuindo
                olamundo.py
                
            }
        }
        stage('Deliver') {
            steps {
                echo 'entregando....'
                
            }
        }
    }
}
