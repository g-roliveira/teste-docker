pipeline {
    agent {
        dockerfile {
            label 'docker-dind'
        }
    }
    post {
        always {
            // Comandos de limpeza que sempre serão executados
            echo 'Executando etapas de limpeza...'
            // Adicione aqui seus comandos de limpeza
        }

        success {
            // Comandos específicos para quando a pipeline for bem-sucedida
            echo 'Pipeline concluída com sucesso!'
        }

        failure {
            // Comandos específicos para quando a pipeline falhar
            echo 'Falha na execução da Pipeline.'
        }
    }    
}
