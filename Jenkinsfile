pipeline {
    agent none

    stages {
        stage('Maven Install') {
            agent {
                docker {
                    image 'maven:3.5.0'
                    label '' // Optional: you can add a label if required for specific nodes
                    reuseNode true // This allows the container to use the same workspace
                }
            }
            steps {
                sh 'mvn clean install'
            }
        }
    }
}