pipeline {
    agent any
  stages {
    stage('Build') {
            steps {
                    sh "sh ./build.sh"
                 }
        }
      stage('Test') {
            steps {
                    sh "sh ./test.sh"
            }
        }
      stage('Deploy') {
            steps {
                    sh "sh ./deploy.sh"
            }
        }
  }
    post {
        always {
            sh 'echo "job finished"'
        }
    }
}
