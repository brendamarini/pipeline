pipeline {
    agent any 

    stages {
        stage('Build') {
            steps {
                echo "construindo....."
                echo "terminado"
            }
        }
        stage('Test') {
            steps {
                echo "testando"
                sh '''
                cd comandos
                ls
                cat requisito
                '''
                echo "teste completo"
            }
        }
        stage('Deliver') {
            steps {
                echo "entregando"
                echo "entrega completa"
            }
        }
    }
}
