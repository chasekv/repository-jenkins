pipeline {
    agent any
    stages {
        stage ('compile stage') {
           steps {
               maven(maven : mvn compile) 
                   sh '''mvn clean compile'''
            }
        }
  }
}
