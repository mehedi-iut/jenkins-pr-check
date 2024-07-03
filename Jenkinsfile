pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from the PR
                checkout scm
            }
        }

        // stage('Install Dependencies') {
        //     steps {
        //         // Install npm dependencies
        //         sh 'npm install'
        //     }
        // }

        stage('Build') {
            steps {
                // Run the build process
                sh 'echo Hello World'
            }
        }
    }

    post {
        success {
            echo 'Build successful! The changes look good.'
        }
        failure {
            echo 'Build failed. Please check the logs and fix the issues.'
        }
    }
}
