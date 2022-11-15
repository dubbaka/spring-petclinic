#!groovy

pipeline {
	agent none
  stages {
  	stage('Which User') {
    	agent any
      steps {
      	sh 'whoami'
      }
    }
    stage('Docker Build') {
    	agent any
      steps {
      	sh 'docker build -t dubbaka/spring-petclinic:latest .'
      }
    }  
}