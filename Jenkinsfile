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
                echo "Building...."
            }
        }

        stage('Static Analysis') {
            steps {
                echo "Analyzing...."
            }
        }

        stage('Unit test') {
            steps {
                echo "..... Unit tests passed"
            }
        }
    }
}
