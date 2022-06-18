pipeline{
    agent any
    stages{
        stage('Git clone'){
            steps{
                git 'https://github.com/manhnghia99/helloworld.git'
            }
        }
        
        stage('maven build'){
            steps{
                sh 'mvn package'
            }
        }
        stage('Create Dockerimage'){
            steps{
                sh 'docker build -t thetips4you/springboot:latest .'
            }
        }
        
    }
}
