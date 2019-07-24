pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                   def mvn = tool 'Maven 3.3.9'
                   sh '${mvn} clean install'
                }    
               
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
