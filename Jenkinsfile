pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                def mvn = tool 'Maven 3.3.9'
                sh '${mvn}\\bin\\mvn clean install'
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
