pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
				sh "curl -X POST --user admin:11b0a151650fa22751ef1f0794a706bbcd http://52.15.252.95:8080/job/APF_PDI/job/main/buildWithParameters?Test=test"
				
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