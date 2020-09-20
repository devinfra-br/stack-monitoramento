pipeline {
    agent any

    stages {
        stage('Validação Docker') {

        // Commands Execute
            steps {
                echo 'Docker Compose Validate'
                sh 'docker-compose -f docker-compose.yml config'
            }
        }
        
        stage('Clone Infra Tools') {
            steps {
                echo 'Teste de Conexão Ansible'
                sh 'rm -rf automation-example'
                sh 'git clone https://github.com/devinfra-br/automation-example.git'
                sh 'cd automation-example'
                sh 'sh iac/bash-scripts/ansible-app-deploy.sh testes server1'
            }
        }

        stage('Execute Ansible') {
            steps {
                echo 'Deploy Stack Monitoramento'
                sh 'cd automation-example'
                sh 'sh iac/bash-scripts/ansible-app-deploy.sh compose'
            }
        }
    }
}
