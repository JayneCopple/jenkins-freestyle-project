pipeline {
    agent any
  stages {
    stage('Build') {
            steps {
                script {
                    sh ./build.sh
                }
            }
        }
      stage('Test') {
            steps {
                script {
                    sh ./test.sh
                }
            }
        }
      stage('Deploy') {
            steps {
                script {
                    sh ./deploy.sh
                }
            }
        }
  }
}
