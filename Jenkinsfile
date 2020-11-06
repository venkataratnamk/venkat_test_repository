pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
				sh "curl -X POST  --url http://52.15.252.95:8080/job/APF_PDI/buildWithParameters --user admin:11b0a151650fa22751ef1f0794a706bbcd --data PERSON=VENKAT --data BIOGRAPHY=SELF"

				
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
		stage ('Invoke_pipeline') {
		steps {
			build job: 'http://52.15.252.95:8080/job/APF_PDI/job/main/', parameters: [
			string(name: 'param1', value: "value1")
			]
		}
}
    }
}