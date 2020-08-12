pipeline{
    agent any
    tools{
        nodejs 'node-10.16.4'
    }

    options{
        timeout(time:2, unit:'MINUTES')
    }

    stages{
        stage('Instalando dependencias'){
            steps{
                sh 'npm i'
            }
        }
        stage('Corriendo Pruebas'){
            steps{
                sh 'npm test'
            }
        }
    }
}