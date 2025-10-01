@Library('shared_library') _

pipeline {
    agent any

    stages {
        stage('Clean') {
            steps {
                script {
                    cleanWorkspace()
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
