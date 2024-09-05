pipeline {
    agent any

    stages {
        stage('Maven Install') {
            steps {
                script {
                    // Run Maven inside a Docker container
                    //docker.image('maven:3.5.0').inside {
                        sh 'mvn clean install'
                   // }
                }
            }
        }
    }
}
