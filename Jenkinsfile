pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
				sh "wget --auth-no-challenge --user=admin --password=11b0a151650fa22751ef1f0794a706bbcd http://52.15.252.95:8080/job/APF_PDI/buildWithParameters?Test=test"
				
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