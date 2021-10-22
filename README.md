pipeline {
    agent any
    stages {
        stage ('compile stage') {
           steps {
               maven(maven: mvn --version) 
                   sh '''mvn clean compile'''
            }
        }
  }
}
