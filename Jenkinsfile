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
                // Ejecutar Maven desde una ruta accesible
                bat 'C:\\apache-maven-3.9.11\\bin\\mvn.bat clean validate'
            }
        }
    }
}







