pipeline {
    agent any

    triggers {
        pollSCM '* * * * *' // Verifica o repositório a cada minuto
    }

    stages {
        stage('Build') {
            steps {
                echo "Construindo..."
                sh 'pip install -r requisitos.txt' // Executa o comando shell para instalar as dependências
            }
        }

        stage('Test') {
            steps {
                echo "Testando..."
                sh 'python3 olamundo.py' // Executa o script Python (certifique-se de que o nome do script está correto)
            }
        }

        stage('Deliver') {
            steps {
                echo 'Entregando....'
                // Adicione os comandos para a etapa de entrega aqui
            }
        }
    }
}
