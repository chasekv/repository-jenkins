pipeline { 
    agent any 
        stages { 
            stage ('Compile') { 
                steps { 
                    sh 'mvn --version' 
                }
            }
        }
    }
