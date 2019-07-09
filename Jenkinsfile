pipeline {
    agent {
        docker {
            image 'maven:3-alpine' 
            args '-v /Users/anhdn19/.m2:/Users/anhdn19/.m2' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}
