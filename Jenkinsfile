pipeline {
    agent any  // Use any available agent

    tools {
        gradle 'Gradle'   // Name must match Jenkins config
        jdk 'JDK'
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'master', url: 'https://github.com/Sandhya-TS203/MyGradleApp01.git'
            }
        }

        stage('Build') {
            steps {
                sh 'gradle build'
            }
        }

        stage('Test') {
            steps {
                sh 'gradle test'
            }
        }
    }
}
