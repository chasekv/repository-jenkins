pipeline {
    agent any

    stages {
        stage ('compile stage') {
        
           steps {
               Maven(maven : 'Maven_3_8_3') {
                   sh 'mvn clean compile'
                }
            }
        }
  }
}
