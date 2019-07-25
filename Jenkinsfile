pipeline {
    environment {
    registry = "viz139/docker_jenkins"
    registryCredential = ‘dockerhub’
    }
    agent any
    stages {
        stage('Build')  {   
           steps {
                script {
                   def mvnHome = tool 'Maven 3.3.9'
                   sh "'${mvnHome}/bin/mvn' clean package"
                }    

            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Build Docker Image')  {   
           steps {
                script {
                   def dockerHome = tool 'docker'
                   sh "'${dockerHome} version"
                }    

            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
