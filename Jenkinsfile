pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
				sh "curl -X POST http://admin:11b0a151650fa22751ef1f0794a706bbcd@52.15.252.95:8080/job/APF_PDI/job/main/buildWithParameters?token=admin"
				
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}