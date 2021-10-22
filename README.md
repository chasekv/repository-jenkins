pipeline {
    agent any

    stages {
        stage ('compile stage') {
        
           steps {
               maven(maven : 'Maven_3_8_3') {
                   sh 'mvn clean compile'
                }
            }
        }
  }
}
