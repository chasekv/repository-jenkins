pipeline {
    agent any
    stages {
        stage ('compile stage') {
           steps {
               maven(maven: mvn) 
                   sh '''mvn clean compile'''
            }
        }
  }
}
