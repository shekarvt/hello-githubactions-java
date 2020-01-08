
pipeline {
  agent any
  stages {
    stage('Build Image s1.0') {
      parallel {
        stage('Build Image s1.0') {
          steps {
            // sh 'sh release/build-docker-images-scenario1.0.sh ${ACR_LOGINSERVER}'
            echo "Build Image s1.0"
          }
        }
        stage('Build Image s1.1') {
          steps {
            // sh 'sh release/build-docker-images-scenario1.1.sh ${ACR_LOGINSERVER}'
            echo "Build Image s1.1"
          }
        }
        stage('Build Image s2.0') {
          steps {
            // sh 'sh release/build-docker-images-scenario2.0.sh ${ACR_LOGINSERVER}'
            echo "Build Image s2.0"
          }
        }
      }
    }
    stage('Push Images ACR') {
      parallel {
        stage('Push Image s1.0') {
          steps {
            // sh 'sh release/push-docker-images-scenario1.0.sh ${ACR_LOGINSERVER}'
            echo "Push Image s1.0"
          }
        }
        stage('Push Image s1.1') {
          steps {
            // sh 'sh release/push-docker-images-scenario1.1.sh ${ACR_LOGINSERVER}'
            echo "Push Image s1.1"
          }
        }
        stage('Push Image s2.0') {
          steps {
            // sh 'sh release/push-docker-images-scenario2.0.sh ${ACR_LOGINSERVER}'
            echo "Push Image s1.1"
            echo "Push Image s1.1"
          }
        }
      }
    }
  }
}
