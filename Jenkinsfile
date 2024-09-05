pipeline {
    agent none // This is fine if you don't want to specify a default agent

    stages {
        stage('Maven Install') {
            agent {
                docker {
                    image 'maven:3.5.0'
                    // Optional: add 'args' here if needed, for example: args '-v /root/.m2:/root/.m2'
                }
            }
            steps {
                sh 'mvn clean install'
            }
        }
    }
}

