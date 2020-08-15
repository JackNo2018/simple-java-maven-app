pipeline {
    agent {
        docker {
            image 'maven:3-alpine'
            args '-v /root/.m2:/root/.m2 -u root --privileged'
        }
    }
    stages {
        stage('Build2') {
            steps {
                sh 'mvn -B clean package'
            }
        }
    }
}