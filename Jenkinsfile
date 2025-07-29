pipeline {
    agent any
    stages {
        stage('checkout') {
            steps {
                git 'https://github.com/BikashPanda1998/jenkins_mvn.git'
            }
        }
        stage('compile') {
            steps {
                sh 'mvn compile'
            }
        }
       stage('package'){
           steps {
                sh 'mvn package'
            }
        }
       stage('install'){
           steps {
                sh 'mvn install'
            }
        }
        stage('sucessfully'){
           steps {
                echo "webhook sucessfully run"
            }
        }
    }
}
