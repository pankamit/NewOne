pipeline {
    agent any

    stages{
        stage('Check Version'){
            steps{
                withMaven(maven : 'Maven 3.6.3') {
                    sh 'mvn -version'
                }
            }
        }
        stage('Compile'){
            steps{
                withMaven(maven : 'Maven 3.6.3') {
                    sh 'mvn clean compile'
                }
            }
        }
        stage('Build'){
            steps{
                withMaven(maven : 'Maven 3.6.3') {
                    sh 'mvn install'
                }
            }
        }
        
    }
    
}