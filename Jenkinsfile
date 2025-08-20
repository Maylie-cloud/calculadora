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
                // Ejecutar Maven usando Windows cmd
                bat "${tool 'm3'}\\bin\\mvn.bat clean validate"

            }
        }
    }
}



