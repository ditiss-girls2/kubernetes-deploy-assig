pipeline {
    agent any

    stages {
		
//	stage('Build Docker Image'){
//            steps{
//                sh 'docker build -t hello-java .'
//            }
//        }
//	stage('Run Docker Container'){
//	    steps {
//		 sh 'docker run :hello-java'
//		}
//	    }
//	
//	stage('Tag Docker Image'){
//            steps {
//                 sh 'docker tag hello-java ditisscdac/hello-java:v1.0'
//                }
//            }
//	stage('Push Docker Image to DockerHub'){
//            steps {
//                 sh 'docker push ditisscdac/hello-java:v1.0'
//                }
//            }
      stage('Build kubernet deployment file'){
            steps{
                sh 'kubectl apply -f kube-deploy.yaml'
            }
        }
       stage('Build kubernet service file'){
            steps{
                sh 'kubectl apply -f kube-service.yaml'
            }
        }


     }
}
