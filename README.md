pipeline {
    agent any
    stages {
        stage ('compile stage') {
           steps {
               maven(mvn compile) {
                   sh 'mvn clean compile'
                }
            }
        }
  }
}
