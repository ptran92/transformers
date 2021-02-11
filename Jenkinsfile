pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo "Clone source code"
            }
        }

        stage('Build') {
            steps {
                sh './ci/build.sh'
            }
        }

        stage('Static Analysis') {
            steps {
                echo "Analyzing...."
            }
        }

        stage('Unit test') {
            steps {
                sh './ci/test.sh'
            }
        }
    }
}
