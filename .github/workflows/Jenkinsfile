pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                sh './gradlew assemble' // TODO: Ensure Gradle build is successful
            }
        }

        stage('Test') {
            steps {
                sh './gradlew test' // TODO: Ensure tests run successfully
            }
        }
    }
}
