pipeline {
    agent any

    stages {
        stage ('compile stage') {
        
           steps {
               maven(maven : 'maven_3_8_3') {
                   sh 'mvn clean compile'
                }
            }
        }
  }
}
