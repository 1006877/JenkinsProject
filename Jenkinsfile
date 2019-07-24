pipeline {
    agent any
    stages {
        stage('Build')  {   
            script {
             def mvnHome = tool 'Maven 3.3.9'
             sh "'${mvnHome}/bin/mvn' clean package"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
