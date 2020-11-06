pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
				curl http://52.15.252.95:8080/job/APF_PDI/job/main/ --user admin:admin --data id=123 --data verbosity=high
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