pipeline {
    agent any
  stages {
    stage('Build') {
            steps {
                script {
                // build script
                    sh ./build.sh
                }
            }
        }
      stage('Test') {
            steps {
                script {
                // test script
                    sh ./test.sh
                }
            }
        }
      stage('Deploy') {
            steps {
                script {
                // deploy script
                    sh ./deploy.sh
                }
            }
        }
  }
}
