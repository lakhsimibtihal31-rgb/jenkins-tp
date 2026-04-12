pipeline {
    agent any
    stages {
        stage('SonarQube Analysis') {
            steps {
                withCredentials([string(credentialsId: 'sonartoken', variable: 'SONAR_TOKEN')]) {
                    sh """
                        echo 'SonarQube Analysis stage'
                    """
                }
            }
        }
        stage('Hello') {
            steps {
                echo 'Hello from Jenkinsfile!'
            }
        }
    }
}
