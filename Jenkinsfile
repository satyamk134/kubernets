pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo "building the heml graphs"
                sh "ansible-playbook deploy.yml  --user=jenkins --extra-vars ImageName=satyamk134/laundary-node-app --extra-vars imageTag=latest --extra-vars Namespace=greentown"
            }
        }
        stage('Test') {
            steps {
                echo "Testing" 
            }
        }
    }
}
