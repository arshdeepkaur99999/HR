
pipeline {
    agent any
 
    tools {
        jdk "JDK"
    }
 
  
    stages {
        stage('git repo & clean') {
            steps {
            
                bat "mvn clean"
            }
        }
        stage('install') {
            steps {
                bat "mvn install"
            }
        }
        stage('test') {
            steps {
                bat "mvn test"
            }
        }
        stage('package') {
            steps {
                bat "mvn package"
            }
        }
    }

 

}
