pipeline {
    tools{
        maven "maven-3.8.7"
    }
    stages {
        stage ("Maven clean"){
            when {
                branch "main"
            }
            steps {
                sh "mvn clean"
            }
        }
        stage("Maven build"){
            when {
                branch "main"
            }
            steps {
                sh "mvn package -DskipTests"
            } 
        }
    }
}