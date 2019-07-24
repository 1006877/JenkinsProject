pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                   def mvn = tool 'Maven 3.3.9'
                }    
                echo "M2_HOME = ${mvn}"
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
