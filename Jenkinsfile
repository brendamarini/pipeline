pipeline {
    agent any 

    stages {
        stage('Build') {
            steps {
                echo "construindo....."
                sh '''
                cd comandos
                ls
                cat requisito
                '''
                echo "terminado"
            }
        }
        stage('Test') {
            steps {
                echo "testando"
                
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
