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
                h "echo 'hi tester' "
            }
        }
        stage('Workspace cleanup') { 
            steps {
                sh "echo 'Cleaning workspace' "
		cleanWs()
            }
        }
    }
}
