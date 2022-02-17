pipeline{
    agent any
    stages{
        stage('Git clone'){
            steps{
                git 'https://github.com/Anil-Jena/HelloWorld-Springboot-App.git'
            }
        }
        
        stage('maven build'){
            steps{
                sh 'mvn package'
            }
        }
        stage('Create Dockerimage'){
            steps{
                sh 'docker build -t anilkumarjena/springboot:latest .'
            }
        }
        
    }
}
