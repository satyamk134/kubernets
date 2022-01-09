pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo "building the heml graphs"
                echo "$USER"
                sh "helm upgrade -i danger-release . --create-namespace  --namespace=greentown"
            }
        }
        stage('Test') {
            steps {
                echo "Testing" 
            }
        }
    }
} 
