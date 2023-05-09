#!groovy
pipeline {
    agent {
        docker {
            image 'maven:latest'
            args '-v /path/to/local/maven/repository:/root/.m2/repository'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
