pipeline {
    agent any

    stages {
        stage ('compile stage') {
        
           steps {
               maven(maven : 'maven3.8.3') {
                   sh 'mvn clean compile'
                }
            }
        }
  }
}
