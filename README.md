pipeline {
    agent any
    stages {
        stage ('compile stage') {
           steps {
               maven(mvn --version) 
                   sh '''mvn clean compile'''
            }
        }
  }
}
