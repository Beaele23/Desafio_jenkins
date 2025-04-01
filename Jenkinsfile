pipeline {
    agent any
    stages {
        stage('Clonar repositorio') {
            steps {
                checkout scm
            }
        }
        stage('Instalar dependencias') {
            steps {
                sh 'npm install'
            }
        }
        stage('Construir imagen Docker') {
            steps {
                sh 'docker build -t sistema-integracion .'
            }
        }
    }
}

