pipeline {
 agent any
 stages {
  stage("git") {
   steps {
   git credentialsId: 'ac7e0575-9485-4e59-b8bb-cff21c407356', url: 'https://github.com/VelpulaAkkini/javaparser-maven-sample.git'
   }
  }
  stage("validate code") {
    steps {
	sh "mvn clean validate"
	}
  }
  stage("compile code") {
   steps {
   sh "mvn clean compile"
   }
  }
  stage("test code") {
  steps {
  sh "mvn clean test"
  }
  }
  stage("package code") {
  steps {
  sh "mvn clean package"
  }
  }
  stage("install code") {
  steps {
  sh "mvn clean install"
  }
  }
}
}
