pipeline{
    agent any
    stages{
        stage('verificar si los navegadores fueron instalados'){
            steps{
                sh 'google-chrome --version'
                sh 'firefox --version'
            }
        }
        stage('ejecutar pruebas'){
            steps{
                sh './mvnw clean test'
            }
        }
    }
}