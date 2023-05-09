#!groovy
pipeline {
	agent none
  stages {
  	stage('Maven Install') {
    	agent {
      	docker {
        	image 'maven:latest'
                args '-v /path/to/local/maven/repository:/root/.m2/repository'
        }
      }
      steps {
      	sh 'mvn clean install'
      }
    }
  }
}
