pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                git changelog: false, poll: false, url: 'https://github.com/nitesh041990/Devops.git'
            }
        }
        stage('Test') { 
            steps {
                sh "echo 'hi tester' "
            }
        }
        stage('Deploy') { 
            steps {
                sh "echo 'test me' "
            }
        }
    }
}
