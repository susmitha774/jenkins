pipeline {
    agent {
        node {
            label 'docker-agent-alpine'  // Make sure this label matches your Docker cloud agent
        }
    }

    triggers {
        pollSCM '*/5 * * * *'  // Polls Git for changes every 5 minutes
    }

    stages {
        stage('Build') {
            steps {
                echo 'Susmitha Manthena - SE22UARI170'
                echo "Stage: Building..."
                sh '''
                echo "Building from Jenkinsfile"
                '''
            }
        }

        stage('Test') {
            steps {
                echo "Stage: Testing..."
                sh '''
                echo "Testing the build triggered from Jenkinsfile."
                '''
            }
        }

        stage('Deliver') {
            steps {
                echo "Stage: Delivering..."
                sh '''
                echo "Doing delivery stuff..."
                '''
            }
        }
    }
}
