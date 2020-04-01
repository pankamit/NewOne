pipeline {
    agent any

    stages{
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