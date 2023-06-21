pipeline {
    agent {
        docker {
            image 'maven:3.9.0-eclipse-temurin-11'
            args '-v C:/Users/satis/.jenkins/workspace/my-first-pipeline_main/:/workspace -v C:/Users/satis/.jenkins/workspace/my-first-pipeline_main@tmp/:/workspace@tmp'
        }
    }
    options {
        // Specify the working directory
        workspace '/workspace'
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}
