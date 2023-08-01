pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                checkout([$class: 'GitSCM', 
                    branches: [[name: '*/main']], 
                    userRemoteConfigs: [[url: 'https://github.com/Toloruntobi/demo-folder.git']]])
            }
        }
        stage('Build') {
            steps {
                // Add build steps here (e.g., Maven or Gradle build)
            }
        }
    }
}

