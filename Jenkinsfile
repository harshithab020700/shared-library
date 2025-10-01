@Library('shared_library') _

pipeline {
    agent any

    stages {
        stage('Clean') {
            steps {
                script {
                    cleanworkspace()
                }
            }
        }
        stage('Welcome') {
            steps {
                script {
                    hello('linux')
                }
            }
        }
        stage('Build') {
            steps {
                script {
                    buildapp()
                }
            }
        }
        stage('Deploy') {
            steps {
                script {
                    deployapp()
                }
            }
        }
    }
}
