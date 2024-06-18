pipeline {
    agent any
        
    
    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage('Build') {
            steps {
                echo "construindo..."
                cd comandos
                pip install -r requisitos.txt
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
                cd constuindo
                python3 olamundo.py
                
            }
        }
        stage('Deliver') {
            steps {
                echo 'entregando....'
                
            }
        }
    }
}
