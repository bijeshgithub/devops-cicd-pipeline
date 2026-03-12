pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t devops-cicd-pipeline .'
            }
        }

        stage('Lists Docker Images') {
            steps {
                sh 'docker images'
             }
        }       
                
        stage ('Deploy to Kubernetes') {
           steps {
               sh 'kubectl apply -f k8s/deployment.yaml'
               sh 'kubectl apply -f k8s/service.yaml'
 
            }
        }

    }
}
