pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
				sh "curl http://52.15.252.95:8080/job/APF_PDI/job/main/buildWithParameters --user admin:11b0a151650fa22751ef1f0794a706bbcd"
				
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