pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    echo 'Building the project...'
                    // Add your build commands here, for example:
                    // sh 'mvn clean install' for a Java project, or npm install for Node.js, etc.
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    echo 'Running tests...'
                    // Add your test commands here, for example:
                    // sh 'mvn test' or npm test, depending on your setup
                }
            }
        }
        stage('Deploy') {
            steps {
                script {
                    echo 'Deploying project...'
                    // Add your deployment commands here.
                }
            }
        }
    }
}
