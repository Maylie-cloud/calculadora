pipeline {
    agent any
    tools {
        jdk 'JDK-11'       // Cambia según tu JDK instalado en Jenkins
        maven 'Maven-3.8'  // Cambia según tu Maven instalado en Jenkins
    }
    stages {
        stage('Checkout') {
            steps {
                // Clonar el repositorio
                git branch: 'main', url: 'https://github.com/Maylie-cloud/calculadora.git'
            }
        }
        stage('Validate Syntax') {
            steps {
                // Ejecutar Maven solo para validar el proyecto
                sh 'mvn clean validate'
            }
        }
    }
    post {
        success {
            echo 'Revisión de sintaxis completada sin errores.'
        }
        failure {
            echo 'Se encontraron errores de sintaxis.'
        }
    }
}
