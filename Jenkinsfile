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
                bat '"C:\\Program Files\\apache-maven-3.9.11\\bin\\mvn.bat" clean validate'
            }
        }
    }
}











