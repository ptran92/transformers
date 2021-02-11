pipeline {
    agent any
    options {
        skipDefaultCheckout()
    }

    stages {
        stage('Clone') {
            steps {
                checkout scm
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
