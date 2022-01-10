pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo "building the heml graphs"
                echo "${params.dockertag}"
                sh "ansible-playbook deploy.yml  --user=jenkins --extra-vars ImageName=satyamk134/laundary-node-app --extra-vars imageTag=${params.dockertag} --extra-vars Namespace=greentea"
            }
        }
        stage('Test') {
            steps {
                echo "Testing" 
            }
        }
        
    }
} 
