pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Maylie-cloud/calculadora.git'
            }
        }
        stage('Validate Syntax') {
            steps {
                // Correcto: comillas simples de Groovy + comillas dobles internas
                bat '"‪C:\Users\Maylie\Downloads\maven-mvnd-1.0.2-windows-amd64'
            }
        }
    }
}












