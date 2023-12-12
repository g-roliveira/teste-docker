pipeline {
    agent {
        label 'dind'
    }
    //agent {
        //dockerfile {
       //     label 'dind'
            // configurações adicionais aqui, se necessário
     //   }
   // }
    stages {
        stage('Hello Docker') {
            steps {
                container('docker') {
                    sh 'docker ps'
                }
            }
        }
    }
    post {
        always {
            echo 'Executando etapas de limpeza...'
            // Comandos de limpeza
        }
        success {
            echo 'Pipeline concluída com sucesso!'
        }
        failure {
            echo 'Falha na execução da Pipeline.'
        }
    }    
}
