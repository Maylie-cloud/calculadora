pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                // Clonar el repositorio
                git branch: 'main', url: 'https://github.com/Maylie-cloud/calculadora.git'
            }
        }
        stage('Validate Syntax') {
            steps {
                // Ejecutar Maven directamente usando PATH
                sh 'mvn clean validate'
            }
        }
    }
}

