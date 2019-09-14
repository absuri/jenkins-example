pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                tool name: 'mvn3.6.1', type: 'maven'
                    sh 'mvn clean compile'    
            }
        }

        stage ('Testing Stage') {

            steps {
                tool name: 'mvn3.5.3', type: 'maven'
                    sh 'mvn test'
                }
        }

         stage ('install Stage') {
            steps {
                tool name: 'mvn3.6.1', type: 'maven'
                    sh 'mvn install'    
            }
        }
    }
}
