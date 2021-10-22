pipeline {
    agent any

    stages {
        stage ('compile stage') {
        
           steps {
               withMaven(maven : 'Maven_3_8_3') {
                   sh 'mvn clean compile'
                }
            }
        }
  }
}
