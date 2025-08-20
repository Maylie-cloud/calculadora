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
                // Ruta de Maven entre comillas simples, sin caracteres invisibles
                bat '\'C:\\Users\\Maylie\\Downloads\\maven-mvnd-1.0.2-windows-amd64\\bin\\mvn.bat\' clean validate'
            }
        }
    }
}













