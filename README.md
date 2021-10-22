pipeline {
    agent any
    stages {
        stage ('compile stage') {
           steps {
               maven(MAVEN_HOME) {
                   sh 'mvn clean compile'
                }
            }
        }
  }
}
