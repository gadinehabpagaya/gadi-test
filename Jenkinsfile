pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
//                 git credentialsId: 'd327a225-bbb2-4a5c-997c-fa0abeb9111e', url: 'https://github.com/gadinehabpagaya/gadi-test.git'
                checkout scm
            }
        }

//         stage('Install Dependencies') {
//             steps {
//                 sh 'pip install -r requirements.txt' // Install project dependencies if needed
//             }
//         }
//
//         stage('Run Tests') {
//             steps {
//                 sh 'python -m unittest test_tests.py' // Run tests using unittest
//             }
//         }

//         stage('Deploy') {
//             steps {
//                 // Add deployment steps if applicable
//             }
//         }
    }

    post {
        success {
            echo 'Pipeline succeeded! Tests passed.'
        }
        failure {
            echo 'Pipeline failed! Tests failed.'
        }
    }
}