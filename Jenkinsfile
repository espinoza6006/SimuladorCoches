pipeline {
    /*
    Pasos para crear un jenkinsfile
    1. Definir my pipelines steps:
        1- clone
        2- compile
        3- test
        4. ...
       
    2. Generar un escuqeleto: Crear un jenkins file syntax con todos los stage que utilizaras...
    3. Completar cada paso y verificar paso a paso.. step by step
    4. mover el script a jenkinksfile
    */
    agent any

    stages {
        stage('Checkout') { // Establecer conecion con un repositorio
            steps {
                git branch: 'master', url:'https://github.com/espinoza6006/SimuladorCoches'
                bat 'dir' 
            }
        }
        stage('Compile') {
            steps {
                dir ('standalone'){ 
                    bat 'dir'
                    bat 'C:/Programs/apache-maven-3.8.6/bin/mvn clean test'
                    }
            }
        }
        stage('Test') {
            steps {
                echo 'Deploying....'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
        
    }
}
