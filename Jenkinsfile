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
                bat 'npm install'
            }
        }
        stage('Construir imagen Docker') {
            steps {
                bat 'docker build -t sistema-integracion .'
            }
        }
    }
}

