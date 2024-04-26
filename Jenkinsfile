pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		                sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm upgrade --install employee-app employee  --set image.repository=https://hub.docker.com/repositories/sriram1406/employee-service --set image.tag=1'
            }
        }
    }
}