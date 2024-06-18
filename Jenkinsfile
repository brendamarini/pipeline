pipeline {
    agent any

    triggers {
        pollSCM '* * * * *' // Verifica o repositório a cada minuto
    }

    stages {
        stage('Build') {
            steps {
                echo "Construindo..."
                cat requisitos.txt
            }
        }

        stage('Test') {
            steps {
                echo "Testando..."
                python3 olamundo.py
            }
        }

        stage('Deliver') {
            steps {
                echo 'Entregando....'
            
            }
        }
    }
}
